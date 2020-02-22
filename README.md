Prune your source file  as necessary (sed, awk etc.).Firstname and surname should be separated
by one blank space.

Run "awk_names" against the edited source file to create a formatted file. Remember to make
 "awk_names"  executable.  The resultant formatted file will contain names from the source file
to be inserted into your mongo database-collection. Add necessary pre-filled fields here and 
allow for a person having multiple names

Create the formatted list of names with:  "/. awk_names | tee add_names.js". Observe folder 
permissions to ensure the creation of the file "add_names.js".

The file "add_names.js" will be the argument to the mongodb-command for communicating with 
your mongo database.

Final command will be: mongo 127.0.0.1/YOUR_DB/add_names.js





