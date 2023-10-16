 Book Bizz Store 
- A Java Web Developement Project

- Admin Login Credentials: (Admin/Admin)
<hr>
![bookbizzLanding page](ht![bookbizzLanding page](https://github.com/mahsan15/BookBizzStore/assets/82739557/de649c22-ba0b-4686-a555-ffcd0a109ccf)
tps://github.com/mahsan15/BookBizzStore/assets/82739557/dca407bd-6a19-4f91-bcd3-f2c7a259b2dd)

![bbregister](https://github.com/mahsan15/BookBizzStore/assets/82739557/fbfe2b27-b41b-44ca-a4b8-3e599fce5f4d)

![bblogin](https://github.com/mahsan15/BookBizzStore/assets/82739557/b7232858-e9b4-4f71-a934-02717d58dfe4)
![bblist](https://github.com/mahsan15/BookBizzStore/assets/82739557/110399a2-15d6-4076-999c-1bf24fb0273f)
![bbcusto![bbcartcheck](https://github.com/mahsan15/BookBizzStore/assets/82739557/0a65b0c2-7c24-4bc7-becf-fd4f21b4cff9)
merlogin](https:/![bbcart](https://github.com/mahsan15/BookBizzStore/assets/82739557/570fbb37-3ad2-46d4-9988-11a32c3e96a4)
/github![bbadminLogin](https://github.com/mahsan15/BookBizzStore/assets/82739557/4739359d-f91f-4049-8ed0-c03df9af1a16)
.com/mahsan15/BookBizzStore/assets/82739557/a6992388-dbe3-4eaa-b532-774a0d88bf39)
![bbabout](https://github.com/mahsan15/BookBizzStore/assets/82739557/c19a61f2-baba-4db8-8910-d1359d23bc6e)



### About

A user-friendly Online Bookstore project in which users can log in or register, view the available books, select books along with their quantity, and buy them. Users can also get payment receipts after successful payment. The project can also be used by the administrator, who can add new books, remove books, increase and decrease the quantity of books, change the price of the books as well as maintain the selling history of books.


<span style="color:blue">**This Website is built for following purpose:-**</span>
- For Selling books online.
- Maintaining books selling history.
- Adding and managing books.
- User Friendly.
- For Implementation of Http Servlets in Java.
- This is a Mini-project developed using Java, Jdbc, And Servlets.

<span style="color:blue">**Admin Have Following Access for this online store site:-**</span>
- Add New Books.
- View Books Available.
- Remove Books.
- Increase Books Amount.

<span style="color:blue">**Users Have Following Access for this online store site:-**</span>
- Create New Account or Register.
- Login.
- View Available Books.
- Select Books to Buy.
- Select Books Quantity.
- Buy Books.
- Get Payment Receipt.

### Technologies used:-
1. Front-End Development:
- HTML
- CSS
- Javascript
- BootStrap

2. Back-End Development:
- Java [JDK 8+]
- JDBC
- Servlet

3. Database:
- MySql

### ================ Software And Tools Required ================
- : Git 
- : Java JDK 8+
- : Eclipse EE
- : Apache Maven
- : Tomcat v8.0+ 
- : MySQL Server
- : MySQL Workbench (optional) 

### ================= Dummy Database Initialization =================

STEP 1: Open MySQL Command Prompt or MySQL Workbench

STEP 2: Login to the administrator user as : ```mysql -u <username> -p``` (Enter Password if asked)

STEP 3: Copy paste the following MySql Commands-
```MySQL
create database if not exists onlinebookstore;

use onlinebookstore;

create table if not exists books(barcode varchar(100) primary key, name varchar(100), author varchar(100), price int, quantity int);

create table if not exists users(username varchar(100) primary key,password varchar(100), firstname varchar(100),
    lastname varchar(100),address text, phone varchar(100),mailid varchar(100),usertype int);

insert into books values('9780134190563','The Go Programming Language','Alan A. A. Donovan and Brian W. Kernighan',400,8);
insert into books values('9780133053036','C++ Primer','Stanley Lippman and Josée Lajoie and Barbara Moo',976,13);
insert into books values('9781718500457','The Rust Programming Language','Steve Klabnik and Carol Nichols',560,12);
insert into books values('9781491910740','Head First Java','Kathy Sierra and Bert Bates and Trisha Gee',754,23);
insert into books values('9781492056300','Fluent Python','Luciano Ramalho',1014,5);
insert into books values('9781720043997','The Road to Learn React','Robin Wieruch',239,18);
insert into books values('9780132350884','Clean Code: A Handbook of Agile Software Craftsmanship','Robert C Martin',288,3);
insert into books values('9780132181273','Domain-Driven Design','Eric Evans',560,28);
insert into books values('9781951204006','A Programmers Guide to Computer Science','William Springer',188,4);
insert into books values('9780316204552','The Soul of a New Machine','Tracy Kidder',293,30);
insert into books values('9780132778046','Effective Java','Joshua Bloch',368,21);
insert into books values('9781484255995','Practical Rust Projects','Shing Lyu',257,15);
insert into users values('demo','demo','Demo','User','Demo Home','42502216225','demo@gmail.com',2);
insert into users values('Admin','Admin','Mr.','Admin','Haldia WB','9584552224521','admin@gmail.com',1);
insert into users values('shashi','shashi','Shashi','Raj','Bihar','1236547089','shashi@gmail.com',2);

commit;

```

### ========== Importing and Running The Project Through Eclipse EE ==========

Step 0: Open Eclipse Enterprise Edition. [Install, if not already installed.]

Step 1: Click On File > Import > Git > Projects From Git > Clone Uri > Paste The Repository Url as: ```https://github.com/shashirajraja/onlinebookstore.git```> Select master Branch > Next > Next > Finish.

Step 2. a: Go inside ```src/main/resources > application.properties``` and update the value of database details as per your usage, like db.driver, db.host, db.username and db.password according to your installed mysql/postgresql admin user credentials.

Step 2.b: Right Click on Project > Run as > Maven Build > In the goals field enter "clean install" > apply > run

Step 2.c: Right Click On Project > Build Path > Configure Build Path > Libraries > Remove and Update Any Libraries if Red Mark Exists > Finish.

Step 3: [Only If Tomcat Server is not configured in Eclipse] : Right Click On Project > Run As > Run On Server > Select Tomcat V8.0 > (Select Tomcat V8.0 Installation Location If Asked) Next > Add onlinebookstore > Finish.

Step 4: In The Server Tab > Double Click On Tomcat Server > Ports > Change The Port Number For Http/1.1 To 8083 > Close And Save.

Step 5: Right Click On Project > Run As > Run On Server > Select Tomcat v8.0 > Next > Add All> Done.

Step 6: Check Running The Site At  <a href="http://localhost:8083/onlinebookstore/">http://localhost:8083/onlinebookstore/</a>

Step 7: Default Username And Password For Admin Is "Admin" And "Admin"


Note:- Considering this as a Sample Project, we have not much considered of web security.



<bold>Thanks a lot,</bold><br/>
                                                                                                  
