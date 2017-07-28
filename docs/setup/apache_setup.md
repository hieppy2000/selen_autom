## Apache setup
* Install apache
   * Configure httpd.config
	  change DocumentRoot “/Users/hiep/www”
	  change <Directory “/Users/hiep/www”
	* change “Options FollowSymLinks Multiviews” to “Options Indexes FollowSymLinks Multiviews”
	* apachectl restart
	* apachectl stop/start

   * Linux:
     * Create folder: /var/www/html/TestResults
     * Create folder: /var/www/html/Images
     * Create folder: /var/www/html/TRFiles
   * Window:
     * Create folder: C:/www/html/TestResults
     * Create folder: C:/www/html/Images
     * Create folder: C:/www/html/TRFiles
   * MAC:
     * /etc/apache2/httpd.conf
     * apachectl start/stop/restart
