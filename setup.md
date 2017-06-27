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

