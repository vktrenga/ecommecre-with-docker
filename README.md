# ecommerce-api


Docker Commends

Create/ Build Docker Image

Syntax :``` docker build --tag <ImageName?> . ```

Ex : ``` docker build --tag e-commerce-api . ```


List Docker Images

Syntax : ``` docker images ```

Run Docker Image

Syntax : ``` docker run  <ImageName?> ```

Ex : ``` docker run e-commerce-api ```

Run Docker Image with Publish

Syntax : ``` docker run --publish 8000:8000  <ImageName?> ```

Ex : ``` docker run --publish 4000:8000 node-docker```

Here 4000 is docker port
8000 is application running port
We will use 4000 to call application changes
