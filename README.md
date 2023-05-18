<center>
<h1> Stock Market </h1>
</center>
<center>
<a href="Java url">
    <img alt="Java" src="https://img.shields.io/badge/Java->=8-darkblue.svg" />
</a>
<a href="Maven url" >
    <img alt="Maven" src="https://img.shields.io/badge/maven-3.0.5-brightgreen.svg" />
</a>
</center>
This project is based on Stock Market that is built with the help of Spring Boot with Java.

---
# Dependencies Used 
* SpringBoot Devtools
* Spring web
* Lombok
* H2 Database
* Spring Data JPA

# Framework Used
* Spring Boot

---

# Language Used
* Java

---

## Data Model

The stock data model is defined in the Stock class, which has the following attributes:
```
stockId :Integer
stockName : String
stockPrice : Double
stockOwnerCount : Integer
stockType : (Enum)
stockMarketCap : (Double) 
stockBirthTimeStamp : LocalDateTime
```

---

## Data Flow

1. The user sends a request to the application through the API endpoints.
2. The API receives the request and sends it to the proper controller method.
3. The controller method makes a call to the method in service class.

4. The method in service class builds logic and retrieves or modifies data from the database, which is in turn given to controller class
5. The controller method returns a response to the API.
6. The API sends the response back to the restaurant.

---

## Functions used :-

### API Endpoints :-

* RequestMapping("/stock")
* PostMapping("/")
* GetMapping("/type/{stockType}")
* GetMapping("abovePrice/price/{price}/lowerData/date/{date}")
* GetMapping("/cap/{capPercentage}")
* PutMapping("/marketCap/{marketCap}/id/{id}")
* PutMapping("/stock/type/id")
* PutMapping("/stock/{id}")
* DeleteMapping("/ownerCount/{count}")

---

## Data structure Used
* ArrayList
```
We have used ArrayList data structure as a database to implement CRUD Operations 
```
---

## Project Summary

The Stock Market is a Spring Boot project using Java as a language to enables basic functionality for managing stock.The project is built with the help of Spring Boot Framework for building production-ready applications and this project also use ArrayList as the data structure to store and manage restaurant data. 

The following project consist of four class i.e; the StockController, the StockService, the StockDao, and the Stock class.
