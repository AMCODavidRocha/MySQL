# MySQL
1. Install MySQL on Local Environment 
    * Download and install MySQL server and MySQL client tools for your operating system:
      + Windows: __(Own PC)__
      + macOS: Use brew install mysql if you have Homebrew. __(AMCO Lap)__  
    * Start the MySQL server and verify the installation.
    * Secure the installation by setting a root password and adjusting security settings (e.g., removing test databases and anonymous users).
    * __Task: Verify the installation by logging into MySQL from the command line:__
      - __mysql -u root -p__
    ![pic](src/img/1.png)
  


![Static Badge](https://img.shields.io/badge/DONE-darkgreen?style=for-the-badge&label=Task%3A%20&labelColor=black)

---

2. Download and Load the Sakila Sample Database
    * Download the Sakila sample database from the official MySQL site.
    * Unzip the Sakila database files
    * Load the database into MySQL: 
      + mysql -u root -p < /path/to/sakila-schema.sql
    * Insert the data into the database:
      + mysql -u root -p sakila < /path/to/sakila-data.sql
    * __Task: Verify the Sakila database was installed successfully by listing the available databases and selecting it:__
      - __SHOW DATABASES;__
      ![pic](src/img/2-1.png)
      - __USE sakila;__ 
      ![pic](src/img/2-2.png)
      ![pic](src/img/2-3.png)

![Static Badge](https://img.shields.io/badge/DONE-darkgreen?style=for-the-badge&label=Task%3A%20&labelColor=black)

---

3. Perform Queries Using the Command Line
    * Execute basic SQL queries on the Sakila database directly from the MySQL command line:
      + Retrieve all actors from the actor table:
        - SELECT * FROM actor;
        ![pic](src/img/3-1.png)
        ![pic](src/img/3-1-2.png)
      + Count the number of films in the film table:
        - SELECT COUNT(*) FROM film;
        ![pic](src/img/3-2.png)
      + Find all customers whose last name is "Smith":
        - SELECT * FROM customer WHERE last_name = 'Smith';
        ![pic](src/img/3-3.png)
    * __Task: Run at least five different queries, including:__
      + __SELECT with JOIN between rental and customer.__
      ![pic](src/img/3-4.png)
      + __GROUP BY and HAVING to find the number of rentals per store.__
      ![pic](src/img/3-5.png)
      + __ORDER BY to sort movies by rental duration.__
      ![pic](src/img/3-6.png)
      ![pic](src/img/3-6-2.png)
      ![pic](src/img/3-6-3.png)
      ![pic](src/img/3-6-4.png)
      ![pic](src/img/3-6-5.png)
      ![pic](src/img/3-6-6.png)

![Static Badge](https://img.shields.io/badge/DONE-darkgreen?style=for-the-badge&label=Task%3A%20&labelColor=black)

---
