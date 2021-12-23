# army_engine
Hello All,
Welcome to Jinesh Repo.

Three ways to use Army_Engine:
1) Using Docker Image
2) Using Docker-Compose 
3) Using XAMPP

-> Using Docker Image
1) Make sure your system have installed Docker
2) Run below two command in your system
  -> First Command:    
  sudo docker run --name jinesh-mysql-app -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=jinesh_db -e PMA_HOST=jinesh-mysql-app -p 3306:3306 -d mysql
  -> Second Command: 
  sudo docker run --link jinesh-mysql-app -p 80:80 -d jineshpatel02/army_engine
3) Wait for 1 to 2 min
4) Open any desired browser and type in URL "localhost".
5) And BOOM internal army_engine is working in your system.

-> Using Docker-Compose
1) Download zip file from this repository.
2) Extract in your system.
3) Go to docker-compose.yml directory and same directory open CMD or Terminal.
4) Make sure docker-compose is installed in your system. If not available in your system then first install it.
5) Run below command in Terminal or CMD
   -> First Command:    
   sudo docker-compose up --build
6) Boom Army_Engine is working.

-> Using XAMPP
1) This is little bit complicated method.
2) First download and extract zip file.
3) Copy all iteams from www folder and paste it in XAMPP htdocs folder.
4) Start XAMPP Apache and MySQL.
5) After open XAMPP PHPMyAdmin page and create database name "jinesh_db".
6) Go to your in XAMPP htdocs folder and "find config.php" file. Open it and change "$host=" value (new value is $host="localhost").
7) Boom it's working.

-> How to use Engine.
When you open engine in browser. Here, index.phh page bottom you have see "Cawl" button.
First you have to click on it and it's redirect to "crawl_url" page. Here, what you want add url in your internal army_engine database. you can add that url in URL input and wait for crawling. After that go back to mail page and search it over there.
