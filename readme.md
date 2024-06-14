**  Run on Local **

python3 -m venv venv
source venv/bin/activate
pip3 install fastapi uvicorn
uvicorn api:app --reload

** Docker Container **

docker build -t myfastapiapp .
docker run -d --name myapi -p 8001:8001 myfastapiapp
http://127.0.0.1:8001/helloworld
