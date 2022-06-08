# hdb create

---

This command create a new table with some columns in it.

After this program, all the other programs shall inside the database we initialized.

## showcase

```bash title="create a new table"
$ hdb create -t table_name -c column1:int column2:string column3:float
```

## explain

---

The "-t" means table and the "-c" means column. They can alse be replaced as "table" and "column". Im still considering make specific tags captial.

Next the columns part will have columns behind. The formatting "column_name:type" means the new column will have the data type after ":" symbol. Currently there are 3 types of data can be stored.

* int
* string
* float

Since the database is still being develope, we hope we can add other data type support in the future.
