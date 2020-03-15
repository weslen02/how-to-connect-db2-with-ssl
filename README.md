# How to connect DB2 with SSL on Windows

Connect DB2 with SSL on Tools > DBeaver and QMF

1. Creates and Download
- 1.1. Create a folder for the files jks:
> The files for SSL are usually provided by the DBA teams, I know how to create, but here is not the focus, as this is not a developer action, so possibly, you already have these files that will be described here, for this document be more objective, as I said, I will abstain from these creations of files  and certificates.

Folder Exemple:
```
mkdir C:\db2_ssl
```

- 1.2. Paste the file *jks* in the folder *db2_ssl* that you geted with the DBA teams

- 1.3. You need to download the jar file of IBM, [click here](https://www.ibm.com/support/pages/db2-jdbc-driver-versions-and-downloads)
Login with an account IBM, and start the download how the image below:

*Download drivers to JDBC*
<img src="https://github.com/weslen02/how-to-connect-db2-with-ssl/blob/master/img/1.3.png" class="center">

- 1.4. Extract the files of file tar.gz

- 1.5 Create the folder for the JARs and copy or cut the files as listed in the image below:

*Cp the files*
<img src="https://github.com/weslen02/how-to-connect-db2-with-ssl/blob/master/img/1.5.png" class="center">

- 1.6 Paste the files in the folder:
> **Note:** I think the license jar is not necessary, but if you found blocker for this, and if you IBMer, I can help you;
otherwise, I'm sorry, but I don't know how can get for this jars for people outside the enterprise.
*Paste the files*
<img src="https://github.com/weslen02/how-to-connect-db2-with-ssl/blob/master/img/1.6.png" class="center">
