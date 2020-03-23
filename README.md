# Spring Boot with JPA Example

ตัวอย่างการสร้าง web service เล็ก ๆ (microservice) ด้วย Spring Boot
โดยใช้ JPA ในการจัดการข้อมูลในฐานข้อมูล

__To run with IntelliJ:__

  * Click to run class `th.ku.bookstoreservicejpa.BookstoreservicejpaApplication`

__To compile and run with Maven:__

```$ mvn spring-boot:run```

__Possible calls:__

1. GET all books
	- http://localhost:8090/book

2. GET specific book with id
	- http://localhost:8090/book/{pid} เช่น
	- http://localhost:8090/book/1
	- http://localhost:8090/book/2
	- http://localhost:8090/book/3

3. POST a book (create using json format)
	- http://localhost:8090/book

```
{
    "name": "Data Science",
    "price": 400
}
```

4. PUT a book (modify using json format)
	- http://localhost:8090/book/5

```
{
    "name": "Data Science",
    "price": 350
}
```

5. DELETE a book
	- http://localhost:8090/book/5



__Jenkins:__

  * Install mvn on machine
  * Install `Maven Integration plugin`
  * Set up JDK and Maven in Global Tool Configuration
