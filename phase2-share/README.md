docker build -t my-lab .

docker run -v .\notebooks:/notebooks --name lab -p 8888:8888 -it my-lab bash -c "./start"

http://127.0.0.1:8888/lab