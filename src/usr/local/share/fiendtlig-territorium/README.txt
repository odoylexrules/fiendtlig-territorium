   There is a little bit of self administration here. Until I've designed a
 framework to accept a list of variables via a YAML file, you'll have to occupy
 roles.d/ with the appropriate protocol related function libraries.

   Each function contains a line referencing which systemd service unit you
 might want it to check. Fortunately, this gives us a chance to use lighttpd,
 instead of apache2. For example, of course.

   Each file will have a self-exmplanatory name that you'll have to copy over.

     user@host:~$ sudp cp /usr/local/share/fiendtlig-territorium/httpd.ipv4 \
      /usr/local/include/fiendtlig/role.d/httpd.ipv4

   I suggest reviewing the function you copied over after doing so. Cross check
 configured port numbers, systemd service units, and possibly configuration file
 references
