~	Nette framework ready docker	~
nginx, php8.1, phpmyadmin, sql8, node, composer
---------------------------------------------------------------

Tutorial:

Run terminal in this folder:
	docker-compose up -d
	docker exec -it php74-container bash
	composer create-project nette/web-project projectName
	chmod 777 projectName/temp/
	chmod 777 projectName/log/
	exit
	docker-compose down

Change Nginx config (nginx/default.conf) root /var/www/project/projectName/www; from projectName to actual project name

then type in terminal:
	docker-compose up -d

~ Website is on localhost:8080
~ Phpmyadmin is on localhost:8000
---------------------------------------------------------------

CZECH:

V teto slozce (v terminalu): 
	docker-compose up -d
	docker exec -it php74-container bash
	composer create-project nette/web-project projectName
	chmod 777 projectName/temp/
	chmod 777 projectName/log/
	exit
	docker-compose down

V configu Nginxu (nginx/default.conf) zmenit:
	root /var/www/project/projectName/www; na skutecne jmeno projektu

V teto slozce (v terminalu):
	docker-compose up -d

a ted by melo vsechno slapat jak ma byt :D

~ web je na localhost:8080
~ myadmin na localhost:8000
