# sudoku-solver-spring
I just duct-tape this app altogether

# Dependencies
```
I tested it on 
> cat /etc/debian_version
> 9.12

sudo apt install libopencv2.4


pom.xml
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-test</artifactId>
  <scope>test</scope>
</dependency>
```

# Running
```
mvn install:install-file -Dfile=lib/opencv-249.jar -DgroupId=org.opencv -DartifactId=opencv -Dversion=2.4.9 -Dpackaging=jar -DgeneratePom=true -DcreateChecksum=true

mvn spring-boot:run

```

# Uploading
```
curl --form "file=@sudoku_ok_2.jpg" http://127.0.0.1:8080/uploadFile
```

# Credits
sudoku solver using opencv source [sudoku-solver - https://github.com/joseluisdiaz/sudoku-solver ](https://github.com/joseluisdiaz/sudoku-solver)
spring boot file upload source [spring-boot-file-upload-download-rest-api-example - https://github.com/callicoder/spring-boot-file-upload-download-rest-api-example ](https://github.com/callicoder/spring-boot-file-upload-download-rest-api-example)
