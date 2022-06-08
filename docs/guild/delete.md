# hdb delete

---

This command delete a row of data inside table

## showcase

```bash title="delete a row"
$ hdb delete table_name where condition
```

## explain

take the table below for example:

| c1 | c2 | c3 |
| :------------- | :------------- | :------------- |
| Item One       | Item Two       | Item Two       |
| Item One       | Item Two       | Item Two       |
| Item One       | Item Two       | Item Two       |
| Item One       | Item Two       | Item Two       |

If we want delete the row one, we can use:

```bash title="delete a row"
$ hdb delete table_name where INDEX=0
```

and then the table will become:

| c1 | c2 | c3 |
| :------------- | :------------- | :------------- |
| 0       | 0       | 0       |
| Item One       | Item Two       | Item Two       |
| Item One       | Item Two       | Item Two       |
| Item One       | Item Two       | Item Two       |

This function is mainly clear the data instead of deleteing it since the dataset should keep the origin size even though we want clear something. If what you want is delete the column, please refer to [hdb alter](./alter.md)
