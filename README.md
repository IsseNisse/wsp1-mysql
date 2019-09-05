# wsp1-mysql

Intro till MySql

## Starta server

 Starta terminalen 
 
 Skriv in följande:
 
    * sudo service mysql restart
    
    * sudo service apache2 restart

## MYSQL

**Setup** 

 Kör 

	 * sudo mysql -u root 
	 
	 
 För att göra ny användare	

	 * GRANT ALL PRIVILEGES ON *.* TO 'username'@'localhost' IDENTIFIED BY 'password';
	
 För att kolla vilka användare som finns 

	 * SELECT DISTINCT User FROM mysql.user;
**Start**

 Kör 

	* mysql -u username -p
	
## Databas

 Kommandon:
 
 Skapa en databas:
 
	* create database "name"
	
 Visa databaser eller tables:
 
	* show "name"
	
 Använd databas

	* use "database name";
	
 Skapa ett table med rader och kolumner:
 
        * create table "name" (id int unsigned auto_increment, primary key (id)) engine=innodb;
	
 Lägg till rad
 
	* alter table "name" add "fält" "typ t.ex. string eller int" "värde (null, not null)";
	
 Visa vad som finns i valt table:

	* describe "table name";
	
 Lägg till något i ett fält i ett table:

	* insert into "table name" (fält t.ex. body) values (värden);
	
 Visa vad som finns i vlat fält:

	* select * from "table name";
