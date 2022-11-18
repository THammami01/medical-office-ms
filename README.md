# Dr. Office MS

## Installation

In order to use the app:

1. Download and install the Windows executable `SGP Setup.exe`
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

## Screenshots

![Screenshot 01](/Screenshots/01.png)
<p align="center">
  <b><i>-- Login --</i></b>
</p>

---

![Screenshot 02](/Screenshots/02.png)
<p align="center">
  <b><i>-- Logging In --</i></b>
</p>

---

![Screenshot 03](/Screenshots/03.png)
<p align="center">
  <b><i>-- Home --</i></b>
</p>

---

![Screenshot 04](/Screenshots/04.png)
<p align="center">
  <b><i>-- Menu --</i></b>
</p>

---

![Screenshot 05](/Screenshots/05.png)
<p align="center">
  <b><i>-- Exporting data --</i></b>
</p>

---

![Screenshot 06](/Screenshots/06.png)
<p align="center">
  <b><i>-- Exported XLS file --</i></b>
</p>

---

![Screenshot 07](/Screenshots/07.png)
<p align="center">
  <b><i>-- Import data modal --</i></b>
</p>

---

![Screenshot 08](/Screenshots/08.png)
<p align="center">
  <b><i>-- Importing data in progress --</i></b>
</p>

---

![Screenshot 09](/Screenshots/09.png)
<p align="center">
  <b><i>-- Change password modal --</i></b>
</p>

---

![Screenshot 10](/Screenshots/10.png)
<p align="center">
  <b><i>-- Switching to second user --</i></b>
</p>

---

![Screenshot 11](/Screenshots/11.png)
<p align="center">
  <b><i>-- Search results --</i></b>
</p>

---

![Screenshot 12](/Screenshots/12.png)
<p align="center">
  <b><i>-- No record found --</i></b>
</p>

---

![Screenshot 13](/Screenshots/13.png)
<p align="center">
  <b><i>-- Filtering settings modal --</i></b>
</p>

---

![Screenshot 14](/Screenshots/14.png)
<p align="center">
  <b><i>-- Add new patient --</i></b>
</p>

---

![Screenshot 15](/Screenshots/15.png)
<p align="center">
  <b><i>-- Update existing patient's data --</i></b>
</p>

---

![Screenshot 16](/Screenshots/16.png)
<p align="center">
  <b><i>-- Delete patient's record --</i></b>
</p>
