# Java CI/CD Demo Project

## Tech Stack

- Java 17
- Spring Boot
- Maven
- Jenkins
- SonarQube
- Docker
- Docker Hub / AWS ECR

---

## Build Application

```bash
mvn clean package
```

---

## Run Application

```bash
java -jar target/java-cicd-demo-1.0.jar
```

---

## Build Docker Image

```bash
docker build -t java-cicd-demo .
```

---

## Run Docker Container

```bash
docker run -d -p 8080:8080 java-cicd-demo
```

---

## Jenkins Pipeline Stages

1. Checkout
2. Maven Build
3. SonarQube Scan
4. Docker Build
5. Docker Push
6. Docker Deploy

---

## Access Application

http://EC2_PUBLIC_IP:8080

---

## Health Endpoint

http://EC2_PUBLIC_IP:8080/health
