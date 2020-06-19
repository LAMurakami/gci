My site by IP Address
[lam1ak.asuscomm.com](http://lam1ak.asuscomm.com/)
Dynamic Domain Name Service subdomain possibly being served by the instance.

This repo contains content in the html folder and an apache2 configuration
that can be implemented with:

 sudo ln -s /var/www/gci/gci_apache2.conf \
 /etc/apache2/sites-available/082_gci.conf

 sudo a2ensite 082_gci
 sudo systemctl reload apache2

If the repo contents are installed in a location other than /var/www
the path in the configuration and in the instuctions would have to be modified.

The gci_archive_rebuild.bash script will Rebuild an archive of /var/www/gci
resources when they change.  It is intended to be run daily with:

 ln -s /var/www/aws/gci_archive_rebuild.bash ???

This would then be picked up by the Daily cron job ???
