# wsp1-mysql

Intro till MySql

## Starta server

 Starta terminalen 
 
 Skriv in följande:
 
   * sudo service mysql restart
    
   * sudo service apache2 restart

## MYSQL

**setup** 

Kör 

	 * sudo mysql -u root 
	 
	 
För att göra ny användare	

	 * GRANT ALL PRIVILEGES ON *.* TO 'username'@'localhost' IDENTIFIED BY 'password';
	
För att kolla vilka användare som finns 

	 * SELECT DISTINCT User FROM mysql.user;

Hitta appache2

	 * cd /etc/apache2/
	 * sudo a2enmod userdir
	 
