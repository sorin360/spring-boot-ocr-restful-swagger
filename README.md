laughing-bear
=============

Spring-boot+SwaggerUI+Tesseract-ocr.

Tesseract
=============

`
brew install tesseract --with-all-languages 
`

`
export TESSDATA_PREFIX=/usr/local/Cellar/tesseract/3.05.01/share/tessdata
`

Mvn
=============

`
mvn spring-boot:run -Dspring.profiles.active=dev -DTESSDATA_PREFIX=/Users/yangboz/git/laughing-bear/src/main/resources/tessdata/
`

MicroService
=============



Swagger UI
=============

http://localhost:8083/api/swagger-ui.html

Curl
=============

`
curl -i -X POST -H "Content-Type: multipart/form-data" -F "file=@raw_ocr.png" http://localhost:8083/api/info/smartkit/orc/tesseract
`

Reference
=============

https://code.google.com/p/tesseract-ocr/

http://tess4j.sourceforge.net/

https://github.com/tesseract-ocr/tesseract/wiki

https://github.com/tesseract-ocr/tessdata

http://www.baeldung.com/swagger-2-documentation-for-spring-rest-api

Know Issues
==============

https://github.com/nguyenq/tess4j/issues/34

