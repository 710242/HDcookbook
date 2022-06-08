# hdb alter

---

This command change the arrangement of columns inside table.

## showcase

```bash title="alter column"
$ hdb alter table_name add column:data_type
$ hdb alter table_name drop column
$ hdb alter table_name modify column data_type
```

## explain

there are three functions to support alter:

* add     : add a new column to table
* drop    : drop exist column in table
* modify  : modify the data type for the column(exist data will change)
