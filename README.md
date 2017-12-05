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

* **Delete all files from filesystem operation:**
*http://localhost:8787/fileUploadApi/deleteAll DELETE*

How to Build and run
-------------

```bash
git clone https://github.com/murygin/rest-document-archive.git
cd rest-document-archive
mvn package
```
For starting the Tomcat based application
```bash
java -jar target/spring-boot-angJs-fileuploader-rest-0.1.0.jar
```
Or
```bash
./mvnw spring-boot:run
```
How to invoke the client application ?
-------------
**http://localhost:8787/index.html**

Directory name where the uploaded files will be stored:
-------------
**spring-boot-angJs-fileuploader-rest/fileStore**

Each file will be stored within individual child folders with a metadata.properties file


