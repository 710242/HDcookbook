# hdb init

---

This command init a database which is alse a folder containing a .hdb/ hidden folder in it.

This .hdb/ folder stores all the tables in it and the path cannot be changed or the program will not consider the outer folder as a database.

## showcase

```bash title="init a new database"
$ hdb init mydb
```

## explain

---

The name after init is the name of the folder. If there exists a folder's name is same as above, it will create one with "copy" as suffix
