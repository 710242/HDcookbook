# Welcome to hdb

hdb is a small database written in c and created by some students in chung cheng unniversity. the main purpose of creating this database is for {--the grades--} having greater understands about c language.  

## Commands

---

* `hdb init` - Initialize a new database.
* `hdb create` - Create a new table.
* `hdb insert` - Insert values to the table.
* `hdb alter` - Alter the arrangement of the table.
* `hdb update` - Update the data in the column.
* `hdb delete` - Delete(clear) the data in the column.
* `hdb rename` - Rename table or column.
* `hdb search` - Search for certain data.

## Project layout

---

    application/
        rent_app.c  # One of the application of the database
        ...         # Other source file
    include/
        hdlib.h     # The file include all dependencies for the code
        ...         # Other .h files
    src/
        hdcli.c     # The main CLI tool that will be installed
        ...         # Some implement functions and uncompleted code
    Makefile        # Makefile for all programs start with "hdb" in src/
    ...             # Other files 
