## Apache setup
* Install apache
   -- config httpd.config
      	DocumentRoot "/var/www/html/TestResults"
	<Directory "/var/www/html/TestResults">

   -- Linux:
	- Create folder: /var/www/html/TestResults
	- Create folder: /var/www/html/Images
	- Create folder: /var/www/html/TRFiles
   -- Window:
	- Create folder: C:/www/html/TestResults
	- Create folder: C:/www/html/Images
	- Create folder: C:/www/html/TRFiles
   -- MAC:
	/etc/apache2/httpd.conf
	apachectl start/stop/restart
