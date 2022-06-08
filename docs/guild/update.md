# hdb update

---

This command update the data in the specific column.

## showcase

```bash title="update data"
$ hdb update table_name set column_name=new_data where condition
```

## explain

---

This is the first time we see "where" tag, let's first dive into it.

Where must be placed after the set tag since we cannot assume how many condition there are after where. The way program read arguments after where is from left to right, for example:

```
$ ... where column1=123 AND column2=456 OR column3=789
```

In this example, program first read "column1=123" and then AND operation record the next argument. We can see this as:

```
$ ... where ((((column1=123) AND column2=456) OR column3=789) ... )
```

By this way, the program will record all condition after the where tag finish. In this kind of operation, we will use multithreading to speed up for the next operating.

After the where tag, this function, update, is to update the exist data in the table. We use set tag to receive the target column name and the data to override the old one.
