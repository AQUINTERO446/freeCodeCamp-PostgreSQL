1) Simple example
```
CREATE TABLE person (
  id INT,
  first_name VARCHAR(50),
  last_name VARCHAR(50),
  gender VARCHAR(7),
  date_of_birth DATE);
```

2) More realistic
```
CREATE TABLE person (
  id BIGSERIAL NOT NULL PRIMARY KEY,
  first_name VARCHAR(50) NOT NULL,
  last_name VARCHAR(50) NOT NULL,
  gender VARCHAR(5) NOT NULL,
  date_of_birth DATE NOT NULL,
  email VARCHAR(150));
```

```
INSERT INTO person (first_name, last_name, gender, date_of_birth,email)
VALUES ('Jake', 'Jones', 'MALE', date '1990-12-31', 'jake@gmail.com');
```
