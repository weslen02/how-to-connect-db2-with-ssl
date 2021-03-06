# How to connect DB2 with SSL on Windows

Connect DB2 with SSL in the tool DBeaver

### Contents
- [1. Creates and Download](#1-creates-and-download)
- [2. Connecting on DBeaver](#2-connecting-on-dbeaver)
- [3. Reference](#3-reference)
- [4. About](#4-about)

## Steps

### 1. Creates and Download
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


### 2. Connecting on DBeaver
- 2.1. Create a DB connection, (Learn More about here](https://github.com/ca-cwds/intake/wiki/Install-DBeaver-and-Connect-to-PreInt-DB2)

- 2.2. Inserting the SSL
> The code below is an example where I change on DB/Schema infos, you need type your information how you created in the your machine.
Test is my database name, and after this, are SSL information.

```
<test>:sslConnection=true;sslTrustStoreLocation=C:\db2_ssl\<my-truststore>.jks;sslTrustStorePassword=<mypasswd>;
```

*DBeaver exemple*
<img src="https://github.com/weslen02/how-to-connect-db2-with-ssl/blob/master/img/2.2.png" class="center">

- 2.3 Import the JARs file

*Importing the JARs file*
<img src="https://github.com/weslen02/how-to-connect-db2-with-ssl/blob/master/img/2.3.png" class="center">


- 2.4 Then just test the connection, if the configuration worked you will receive the message *Connected*
<img src="https://github.com/weslen02/how-to-connect-db2-with-ssl/blob/master/img/2.4.png" class="center">



### 3. Reference
Last access 2020-03-13.
- [Install DBeaver and Connect to PreInt DB2](https://github.com/ca-cwds/intake/wiki/Install-DBeaver-and-Connect-to-PreInt-DB2)

- [Configuring Secure Sockets Layer (SSL) support in a Db2 instance](https://www.ibm.com/support/knowledgecenter/SSEPGG_11.1.0/com.ibm.db2.luw.admin.sec.doc/doc/t0025241.html)

### 4. About
This is not a reference document, but it aims to share knowledge, you can help improve it, I know that the english applied here is not the best, I'm brazilian and I'm learning this new language, so if you find mistakes, I apologize, and also I ask you to do a Fork and help me to improve this document so that other people can better understand it and so maybe solve a blocker.

> **Together**, *we can* do more through the IT!

<img src="https://github.com/weslen02/end-img/blob/master/tks.png" class="center">

by:

<img src="https://github.com/weslen02/end-img/blob/master/assWeslen2.png" class="center">


> A good **knowledge** is **shared knowledge**!
