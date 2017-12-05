# File-Store-Project
File upload and retrieval Spring Boot Rest based Service.
=====================

A simple file system based archive with REST interface. An angularJS based web client is also included to test the service.

The available Restful APIs as follows:

* **Upload a file operation:**
*http://localhost:8787/fileUploadApi/uploadfile?file={file} POST*

* **Retrive a file from filesystem by file id operation:**
*http://localhost:8787/fileUploadApi/file/{uuid} GET*

* **Retrieve all files from store operation:**
*http://localhost:8787/fileUploadApi/getallfiles GET*

* **Delete all files from filesystem operation:
*http://localhost:8787/fileUploadApi/deleteAll DELETE*

How to Build and run
-------------

```bash
git clone https://github.com/murygin/rest-document-archive.git
cd rest-document-archive
mvn package
java -jar target/rest-document-archive-0.1.0.jar
```
