# Open source projects details

---

## Big Projects

---

### [NASA Turbofan Microservice](https://github.com/arezamoosavi/predictive-maintenance-microservice)

**Detail:** This app is a microservicce that is developed with Nameko and has these components:

- First based on the data sets in Kaggle, the random forest model is trained to predict remained life cycle in current state of turbine
- A restful service to get turbofan current state data; is developed with Fastapi and built with docker; for load balancing Treafik is employed
- A nameko service that check the data with trained random forest classifier; if the data is faulty or not
- A nameko service that save results and data into HBASE
- Another nameko service that produce data and results into a Kafka topic
- An ELK dashboard is developed to get visualisation for the state of turbofan data
- All these service communicate using RabiitMQ

**Tools:** Docker, Nameko, Hbase, Kafka, ELasticsearch, Logstash, Kibana, Fastapi, Treafik, Random-forest

- [Kaggle](https://www.kaggle.com/arezamoosavi/nasa-predictive-maintenance-notebook)
- [Medium](https://medium.com/@sdamoosavi/ml-microservice-with-nameko-to-implement-a-predictive-maintenance-application-f59d4ed60be3)

---

### [Real-time Fraud Detection](https://github.com/arezamoosavi/FraudDetction-API)

**Detail:** In this project, a trained model in core of web service is used for classification the sent data:

- Based on Credit Card data in Kaggle a random forest classifier is trained
- Both restful service and a websocket connection is developed with Fastapi; in order to process the data
- The results and the data are saved into Cassandra
- This app is built and deployed with docker

**Tools:** Docker, Fastapi, Random Forest Model, Websocket, Cassandra

- [Kaggle](https://www.kaggle.com/arezamoosavi/credit-card-fraud-detection)
- [Medium](https://medium.com/@sdamoosavi/real-time-fraud-detection-web-application-3b99aa85eea8)

---


### [ATM Data Stream Processing](https://github.com/arezamoosavi/3doors)

**Detail:** In this app after start the atm data will be produced into kafka, then using spark streaming the data from that topic in kafka will be parsed and cleaned and saved into potgresql and hdfs; also the spark streaming job will be run with Airflow dag and the whole app is developed and deployed with docker and docker-compose

**Tools:** Airflow, Docker, Spark, Kafka, PostgresSql, HDFS

---

### [Stock Data Analysis](https://github.com/arezamoosavi/stock-troy)

**Detail:** In this app the price of Tesla stock is going to obtained and saved into hdfs every hour and at the end of the day a random forest model is going to be trained to predict next day prices based on history prices; the model also is going to be saved into MinIO. All these tasks is developed on Airflow and built and deployed with docker. At end there is a bokeh app the plot history of prices and uses the model in minio to get next day price in real-time!

**Tools:** Docker, Airflow, Spark, Minio, Bokeh, HDFS, Random-Forest

---

### [Bitcoin Predictor](https://github.com/arezamoosavi/hot-coin)

**Detail:** This app will collect real-time price of bitcoin in USD and save data into csv and every 12h the model for bitcoin value prediction is going to be trained; these tasks are implemented with Twisted; finaly the result is ploted with Bokeh and have api with Tornado. This app is developed and deployed with docker on Heroku.

**Tools:** Docker, Heroku, Tornado, Twisted, Bokeh, Random-Forest

- [Heroku](http://hot-coin.herokuapp.com)
- [Medium](https://medium.com/@sdamoosavi/real-time-bitcoin-monitoring-and-prediction-with-bokeh-and-twisted-205f0d492df0)

---

### [Secret Chat App](https://github.com/arezamoosavi/whisper-chat)

**Detail:** This chat application could have as many users and rooms, that never stores data; it has been develeped with Fastapi websocket; built and deployed with docker on Heroku.

**Tools:** Fastapi, Docker, Websocket, Heroku

- [Heroku](https://wisp.herokuapp.com/docs)
- [Medium](https://medium.com/@sdamoosavi/chatroom-development-with-fastapi-websocket-1c96880412d7)

---

### [Face Analyzer App](https://github.com/arezamoosavi/deepface-app)

**Detail:** The Deepface library is deployed with Fastapi to check and compare faces; it uses mongodb as db and developed and deployed with docker on Heroku.

**Tools:** Docker, Tensorflow, Deepface, Fastapi, Mongodb, Heroku

- [Heroku](https://deepface-app.herokuapp.com/docs)
- [Medium (1)](https://medium.com/@sdamoosavi/deploy-deepface-model-fastapi-develop-2e33374db6f2)
- [Medium (2)](https://medium.com/@sdamoosavi/deploy-deepface-model-fastapi-heroku-deployment-8e007e72c455)

---

### [Music Recommender Restful Api](https://github.com/arezamoosavi/rec-music)

**Detail:** Music recommender with Item based collaborative filtering based on KNN:

- The Restful service is developed with Fastapi
- This app is built and deployed with docker on Heroku

**Tools:** Docker, Fastapi, Pandas, Scikit-learn, Heroku

- [Heroku](https://rec-music.herokuapp.com/docs)
- [Medium](https://medium.com/@sdamoosavi/deploy-music-recommender-on-heroku-e0dce3d924ef)

---

### [Goodreaders Book Recommender](https://github.com/arezamoosavi/book-recommend-web-service)

**Detail:** Book Recommender with Item based collaborative filtering based on KNN (based on kaggle dataset):

- The Restful service is developed with Flask and ML tasks is handeled with celery
- Cassandra is database for saving results and data
- This app is built and deployed with docker

**Tools:** Cassandra, Flask, Restful-api, Pandas, Scikit-learn, Gunicorn, Redis, RabbitMq, Celery, Docker

- [Medium (1)](https://medium.com/@sdamoosavi/book-recommender-web-service-ml-e79119535258)
- [Medium (2)](https://medium.com/@sdamoosavi/book-recommender-web-service-cassandra-4a359917d713)
- [Medium (3)](https://medium.com/@sdamoosavi/book-recommender-web-service-flask-and-celery-18c8245a257e)

---

### [Spotify Music Recommender](https://github.com/arezamoosavi/music-recsys-engine-app)

**Detail:** Music recommender with Item based collaborative filtering based on KNN:

- The Restful service is developed with Flask and ML tasks is handeled with celery
- Postgres is database for saving results and data
- This app is built and deployed with docker

**Tools:** Flask, Pandas, Postgres, Docker, Nginx, Celery, Rabbitmq, Redis

- [Medium (1)](https://medium.com/@sdamoosavi/music-recommender-web-service-flask-and-celery-a1274b488ab)
- [Medium (2)](https://medium.com/@sdamoosavi/music-recommender-web-service-ml-ef6fdd1fc026)

---

### [Movie Recommender](https://github.com/arezamoosavi/movie-recommendation)

**Detail:** Movie recommender with Item based collaborative filtering based on KNN (based on movielens data):

- The Restful service is developed with Flask and ML tasks is handeled with celery
- Mongodb is database for saving results and data
- This app is built and deployed with docker

**Tools:** Flask, Pandas, Mongodb, Docker, Nginx, Celery, Rabbitmq, Redis

- [Medium (1)](https://medium.com/@sdamoosavi/movie-recommender-web-service-ml-ce6d11d1d13f)
- [Medium (2)](https://medium.com/@sdamoosavi/movie-recommender-web-service-flask-and-celery-bc792e254a4a)

---

### [Microservice App with Flask and Fastapi deployed using K8S](https://github.com/arezamoosavi/micro-telesys)

**Detail:** A simple microservice implemnted with Nameko, Fastapi and Flask; built with docker and deployed using Kubernetes

**Tools:** Nameko, RMQ. Redis, Flask, Fastapi, Docker, Kubernetes

- [Medium (1)](https://medium.com/@sdamoosavi/nameko-microservice-with-flask-and-fastapi-docker-6e9230408ad1)
- [Medium (2)](https://medium.com/@sdamoosavi/nameko-microservice-with-flask-and-fastapi-kubernetes-a51f83d39b01)

---

## Small Projects and Practices:

---

### [APIs Load Testing](https://github.com/arezamoosavi/Api-load-testing)

**Detail:** Hands on Load Testing with Locust; This app is restful service developed with Starlette and Postgres as database. All services are built and deployed using docker.

**Tools:** Kafka, Faust, Locust, Starlette, Asyncpg, tortoise, redis, Docker

- [Medium](https://medium.com/@sdamoosavi/web-application-load-testing-with-locust-c532f2f5b3eb)

---


### [Simple Web App k8s deployment](https://github.com/arezamoosavi/minium)

**Detail:** A simple rest service with Fastapi; dockerized and deployed with k8s

**Tools:** Fastapi, Kubernetes, Docker, Docker-registery

- [Medium](https://medium.com/@sdamoosavi/part1-deploy-a-simple-web-application-with-kubernetes-2c02c571aacb)

---

### [Another with App k8s deployment](https://github.com/arezamoosavi/INapp)

**Detail:** A simple web service that uses posgres is developed with Fastapi on docker and deployed with k8s

**Tools:** Docker, Docker-registery, Fastapi, Postgresql, Tortoise-orm, Asyncpg, Kubernetes

- [Medium](https://medium.com/@sdamoosavi/part2-deploy-a-more-complex-web-application-with-kubernetes-dc6ea2ad6c8d)

---

### [Nameko App k8s deployment](https://github.com/arezamoosavi/wubba)

**Detail:** Just a simple microservice developed with Nameko and deployed with k8s

**Tools:** Docker, Nameko, Redis, RabbitMQ, Kubernetes

- [Medium](https://medium.com/@sdamoosavi/part3-deploy-a-cqrs-microservice-with-kubernetes-7780f6a26631)

---


### [ELK stack](https://github.com/arezamoosavi/citro-m)

**Detail:** The data is produced into a topic in kafka, the with logstash configuration; the data will be stored in elasticsearch and using kibana a dashboard could be developed. This add is build and deployed with docker

**Tools:** Kafka, Logstash, Elasticsearch, Kibana, Docker-compose

- [Medium](https://medium.com/@sdamoosavi/real-time-data-monitoring-using-kafka-logstash-elasticsearch-and-kibana-39eb046d214f)

---

### [Mock for Testing Faust Streaming](https://github.com/arezamoosavi/f-on-top)

**Detail:** A simple Faust stream processing app and how to mock the asynchronous process of Faust for unit tests; also mocking mongodb. This app is built with docker.

**Tools:** Faust, Mongodb, Mock, Unit tests, Kafka, Docker

- [Medium](https://medium.com/@sdamoosavi/mocking-for-unit-testing-in-faust-application-and-mongodb-ae40b31e0832)

---

### [Real-time Dashboard](https://github.com/arezamoosavi/puiiter)

**Detail:** A dashboard for the gold price data in mysql using grafana; also monitoring kafka and the topics data rate.

**Tools:** Prometheus, Grafana, Mysql, Kafka, Docker

- [Medium](https://medium.com/@sdamoosavi/real-time-data-monitoring-with-grafana-2e9d0a51f55)

---

### [Real-time Bitcoin Price](https://github.com/arezamoosavi/BTC-Alarming)

**Detail:** Every Second the Bitcoin value is going to get processed and saved into postgres, if the value goes under a specific pre-defined value; it will alarm. This app is built and deployed with docker.

**Tools:** Faust, Kafka, Asyncpg, Tortoise, Docker, Redis

- [Medium](https://medium.com/@sdamoosavi/real-time-bitcoin-notification-with-faust-f8fc32490fa5)

---

### [ETL With Cassandra](https://github.com/arezamoosavi/ETL-Cassandra)

**Detail:** In this app:

- The goggle stock data is saved into cassandra using cqlengine
- Then an ETL job will take the data and after preprocessing, using them to predict next month closing price
- This app is built and deployed using docker.


**Tools:** Cassandra, Pandas, Scikit-learn, ETL, Docker

- [Medium](https://medium.com/@sdamoosavi/google-stock-data-etl-with-cassandra-and-predictive-modeling-with-it-756a56b49ea9)

---

### [Transfer Learning Application](https://github.com/arezamoosavi/circus_of_orchestra)

**Detail:** Implementation of training, pre-trained keras and torch models for categorical datasets; this app is built using docker.

**Tools:** Docker, Tensorflow, Torch, Keras

---


### [GPS Data Stream Processing](https://github.com/arezamoosavi/bluebus)

**Detail:** Streams of GPS data are produced into kafka; using spark-streaming the data will be analyzed and stored into postgres; This app is built and deployed with docker.

**Tools:** Docker, Kafka, Spark, Postgres

---

### [Benchmarking Web Frameworks](https://github.com/arezamoosavi/web-services-bench)

**Detail:** Implementation of very simple web applications and trying to do some stress tests; all apps are built and deployed with docker.

**Tools:** Docker, Django, Flask, Fastapi, Falcon, Rust, Go

---

### [Jupyter k8s Deployment](https://github.com/arezamoosavi/tpum-service)

**Detail:** Deployment of Jupyterlab using dockerhub and K8S.

**Tools:** Centos7, Kubernetes, Jupyter, Docker

- [Medium](https://medium.com/@sdamoosavi/deploy-jupyter-lab-with-kubernetes-135f54e04da)

---

### [Hands on Spark with Scala](https://github.com/arezamoosavi/fpianeska)

**Detail:** Hands on Spark using scala and sbt. All process is built and deployed with docker.

- Hands on movilens data: ALS algorithm for movie recommendation, Spark SQL on data and etc.

**Tools:** Spark, Scala, Docker

---

### [Dashboards with druid superset](https://github.com/arezamoosavi/glasco)

**Detail:** Hands on Kafka, Druid, Superset; for dashboards. All services are built and deployed using docker.

**Tools:** Kafka, Druid, Superset, Docker

---

### [Simple Rust Web app and K8S deployment](https://github.com/arezamoosavi/getRusty)

**Detail:** A very simple rest api app developed with rust; using docker for building and Kubernetes for deployment.

**Tools:** Rust, Docker, Kubernetes

---


### [Scala and Java Apps on Docker](https://github.com/arezamoosavi/oldSchool)

**Detail:** Developing Java and Scala apps using docker.

**Tools:** Scala, Java, Docker

---

### [Databases scripts](https://github.com/arezamoosavi/client-side-datasources)

**Detail:** Hands on Mysql, Mongodb, Postgres, MSSQL using python and jupyter. All services are built and deployed using docker.

**Tools:** Mysql, Mongodb, Postgres, MSSQL, Docker

---

### [Store App with Graphql](https://github.com/arezamoosavi/shopping-app)

**Detail:** An store application:

- Developed with django rest framework (DRF) and using Graphene for Graphql routes
- This app is built and deployed using docker

**Tools:** Django Rest Framework, Postgre, Docker, Graphiql, Graphene

- [Medium](https://medium.com/@sdamoosavi/shopping-application-with-django-and-django-graphene-7b47e9d1bf7a)

---

### [Spam Classifier](https://github.com/arezamoosavi/shopping-app)

**Detail:** Quora Duplicate Question Classifier on XGBOOST with 81% accuracy

**Tools:** Xgboost, Pandas, Scikit-learn

- [Kaggle](https://www.kaggle.com/arezamoosavi/quora-duplicate-detection)

---

### [Topic Modeling](https://www.kaggle.com/arezamoosavi/consumer-complaints-prediction)

**Detail:** Predicting Consumer Product based on Consumer‘s Complaints with 98% accuracy

**Tools:** Keras, Pandas, Tensorflow

- [Kaggle](https://www.kaggle.com/arezamoosavi/consumer-complaints-prediction)

---

