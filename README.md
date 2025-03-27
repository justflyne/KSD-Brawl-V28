# KSD Brawl V28

# Как запустить?

  # 1. Скачайте dotnet 8.0 на свой VPS:  
  
    sudo apt-get update && \
      sudo apt-get install -y dotnet-sdk-8.0
  
  # 2. Скачайте на ваш VPS MySQL:
  
  sudo apt update
  sudo apt install mysql-server -y
  sudo mysql_secure_installation 
  тут делаете конфиг для своего бд, лень дальше писать
  
  `Use Google`
  
  # 3. Импортируйте файл `database.sql` из репозитрия в вашу базу

  mysql -u root -p
  CREATE DATABASE имябд;
  USE имябд;
  SOURCE database.sql;
  exit
  
  # 4. Подключите базу-данных к серверу
  Укажите данные своей базы-данных по пути `Supercell.Laser.Server/config.json` в файле `config.json`
     
  # 5. Откройте папку Supercell.Laser.Server:
     cd Supercell.Laser.Server
  
  # 6. Запустите сервер:
     dotnet run
     
  # 7. Ну тут вроде всё должно запуститься и работать
  а если чето не работает сами решайте
