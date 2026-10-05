mkdir Second 
cd  Second 

nano Dockerfile (insert the dockerfile code) 

mkdir src 
cd src 


nano index.js(insert the index.js code) 
cd .. 

sudo apt-get update 
sudo apt install npm

npm init -y 
npm install express 


nano package.json 

remove the text and add theses two lines after the script 
"start": "node dist/index.js",
    "build": "mkdir -p dist && cp -r src/* dist/"

    
npm install 
npm run build
npm start

then check the localhost and create a dockerimage in cmd 


sudo docker build -t NEW .

sudo docker images 



create a container from the image NEW 
sudo docker run -d -p 3000:3000 --name OLD NEW   (OLD is the container name ) 


sudo docker container ls 

