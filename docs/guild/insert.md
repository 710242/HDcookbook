# hdb insert

---

This command insert the data into table in the arrange of columns.

## showcase

```bash title="insert data into table"
$ hdb insert into table_name values for_column1 for_column2 ...
```

## explain

---

In the command line, the data after "values" tag will be arranged into the data for columns. If the length of data is not as same as the column's length, the error of wrong length will be occured.
