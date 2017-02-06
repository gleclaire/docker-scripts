

docker build -t gleclaire/rails:2.0 .

docker run -d -i --name rails -v "$HOME":/usr/src/app -p 3000:3000 -w /usr/src/app gleclaire/rails:2.0 

docker exec -it rails bash

cd gitProjects/myproject/
bundle install
