# ERD03

## 1. Entities

- car
- engine 
- tire
- customer
- engineFactory
- supplier
- battery
- tireFactory
- cylinder

## 2. Attributes

### car
- type
- price

### engine
- powerRating

### tire
- brandName

### customer
- name

### engineFactory
- location

### supplier
- supplierCode

### Battery
- capacity

### tireFactory
- brand name

### cylinder
- volume

## 3. Relations
- a `car` has **exact one** `engine`
- a `car` has **one or zero** `batteries`
- a `car` has **one or zero** `customers`
- a `car` has **many** `tires`
- an `engine` **has one or zero** `cars`
- an `engine` has **exact one** `engineFactory`
- an `engine` has **zero or many** `cylinders`
- a `tire` has **one or zero** `cars`
- a `tire` has **exact one** `tireFactory`
- a `customer` has **one or many** `cars`
- an `engineFactory` has **one or many** `engines`
- a `supplier` has **one or many** `cylinders`
- a `battery` has **one or zero** `cars`
- a `tireFactory` has **one or many** `tire`
- a `cylinder` has **one or zero** `engines`
- a `cylinder` has **exact one** `supplier`



## 4. Cardinalities

- (car, engine) **=> 1:c**
- (car, battery) **=> c:c**
- (car,  customer) **=> c:m**
- (car, tire) **=> m:c**
- (cylinder, engine) **=> c:mc**
- (cylinder, supplier) **=> 1:m**
- (tire, tireFactory) **=> 1:m**
- (engineFactory, engine) **=> m:1**

## 4a. ERD Diagram with yEd

<img src ="/Users/quirin/Documents/3AHITM/Informationssysteme/Uebungen/ERD03/erd03.png">





