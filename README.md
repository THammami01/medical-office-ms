# Dr. Office MS

## Installation

In order to use the app:

1. Download and install the Windows executables `SGP Setup.exe`
2. Install MySQL or MariaDB and create a database with the following requests:

```sql
CREATE DATABASE `SGP`;

CREATE TABLE `SGP`.`User`(
  userNb INT PRIMARY KEY AUTO_INCREMENT,
  userId VARCHAR(255) NOT NULL UNIQUE,
  userPwd VARCHAR(255) NOT NULL
);

INSERT INTO `SGP`.`User`(userId, userPwd)
VALUES("MK", "12345678"), ("AN", "12345678");

CREATE TABLE `SGP`.`Patient`(
  patientNb INT PRIMARY KEY NOT NULL,
  patientId VARCHAR(255) NOT NULL UNIQUE,
  lastname VARCHAR(255) NOT NULL,
  firstname VARCHAR(255) NOT NULL,
  nicNb VARCHAR(255) NOT NULL,
  phoneNb VARCHAR(255) NOT NULL,
  birthday VARCHAR(255) NOT NULL,
  addday VARCHAR(255) NOT NULL,
  parentName VARCHAR(255) NOT NULL
);

INSERT INTO `SGP`.`Patient` VALUES(
  1, "0001", "Y", "X", "09000001", "(+216) 97 000 001", "30/11/1991", "11/08/2021", "X' Y'"
);
```

3. Verify the connection strings: `DB_HOST`, `DB_PORT`, `DB_USER`, `DB_PASSWORD`, and `DB_DATABASE`
4. Run `SGP.exe`
