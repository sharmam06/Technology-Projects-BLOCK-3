# Understanding File Permissions

## Task 1 --- Create a File

Run:

    touch secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)

### Questions

1.  Who owns the file?
-Root owes the file.
2.  What are the default permissions?
-The owner can read and write while group members and other users  can only read the file. 

### Reflection

Why is file ownership important in Linux systems?
-Because it controls who can access, read,write or modify files.It helps protect sensitive information, prevent unauthorised changes and maintain system security.

------------------------------------------------------------------------

## Task 2 --- Restrict File Permissions

Run:

    chmod 600 secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)

### Questions

1.  Who can read the file now?
-The owner
2.  Who cannot access it?
-Group and the other users 


------------------------------------------------------------------------

## Task 3 --- Open Permissions (Security Risk)

Run:

    chmod 777 secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)

### Questions

1.  Who can access the file now?
-Everyone
2.  Why might this configuration be dangerous?
-Loss of Confidentiality
-Tampering and data Corruption.
