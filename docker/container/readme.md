    1  apt-get update
    2  apt-get install curl -y
    3  curl
    4  curl -sL https://deb.nodesource.com/setup_10.x | bash
    5  apt-get install nodejs -y
    6  
   12  cd opt
   13
   15  mkdir node-app
   17  cd node-app/
   18  echo 'console.log("nodejsapp from ubuntu");' >index.js
   19  ls
   20  node index.js
   21  history