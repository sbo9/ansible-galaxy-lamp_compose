Role Name
=========

Téléchargement de apache2, mariadb-server et phpmyadmin. Donne accès à Wordpress sur le localhost.

Requirements
------------

Veillez à ce que vos ports 80, 3306, 8080 soient libres (ports utilisés par défaut).

Role Variables
--------------

Les variables du rôle se définissent dans vars/main.yml
Les variables sont :
			- database 		 : 	wordpress					-	 database par défaut
			- repertoire_projet 	 :	 /ost						- 	 répertoire du projet (volume partagé) par défaut
			- user 			 :	wordpress  					-	 nom d'utilisateur par défaut pour accéder à la database
			- password		 : 	secret						-	 mot de passe par défautpour accéder à la database
			- ports			 :	80 (apache), 8080 (phpmyadmin), 3306 (mariadb)	-	ports de redirection par défaut

Dependencies
------------

Aucunes.

Example Playbook
----------------

    - hosts: servers
      roles:
         - lamp_compose

License
-------

BSD

Author Information
------------------

S. B.
