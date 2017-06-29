<h1>How to make the configuration file for MongoDB(for Windows)</h1>

1. Press the Windows key and type "cmd."

2. Press CTRL+SHIFT+ENTER to open the command prompt in administrative mode.

3. echo.>mongod.cfg

4. Now you need to open up the file. Type: start notepad mongod.cfg

5. Add this information: 
systemLog:
    destination: file
    path: c:\data\log\mongod.log
storage:
    dbPath: c:\data\db

6. Save and close.

<h1>How to open and close MongoDB(for Windows)</h1>

1. Press the Windows key and type "cmd."

2. Press CTRL+SHIFT+ENTER to open the command prompt in administrative mode.

3. Type this to open MongoDB: net start MongoDB 

4. Type this to close MongoDB: net stop MongoDB


<h1>To Import Files Into MongoDB</h1>

<b>Note: Make sure your file has the appropriate file ending before trying to import!!! In addition, make sure that the file is in the same location as mongoimport.</b>

1. Type mongoimport --db "database name" --collection "collection name" --type "file type" --file "Filename"
Note: you don't need to put the database name or collection name in quotes. If you are entering the whole directory path(ex. C:\Program Files\MongoDB\....), then you need to put it in quotatation marks.

<h1>To Start Up The MongoDB Shell From Scratch</h1>

1. Press the Windows key and type "cmd."

2.  Press CTRL+SHIFT+ENTER to open the command prompt in administrative mode.

3. Type <i>net start MongoDB</i> to open Mongo DB.

4. Make sure to change your directory to the location where mongo.exe is located.

5. Type <i>mongo.exe</i> to start the mongo shell.

