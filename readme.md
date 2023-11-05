# Investify App

Investify App is a cutting-edge financial tool designed to make saving and investing an engaging and interactive experience. With a focus on building savings habits, the app integrates gamification with practical financial services.

## Getting Started

### Building From Scratch

To set up your environment: 

1. Create a MySQL database with the following credentials provided in a `.env` file for each service:  

```plaintext
DB_HOST=54.210.73.216
DB_USER=pknadimp
DB_PASSWORD=1234
DB_NAME=Money
```  

2. Build your Docker image using the command:

```shell
docker build -t <desired_name> .
```  

### Using Pre Build Services  

Avatar Service:
```shell
docker pull pknadimp/avatar_svc
docker run -d -p 5050:5050 pknadimp/avatar_svc
```  

Challenge Generator Service:
```shell
docker pull kasyap1/challenge_generator
docker run -d -p 5002:5002 kasyap1/challenge_generator
```  

Leaderboard Service
```shell
docker pull pknadimp/leaderboard_svc
docker run -d -p 5001:5001 pknadimp/leaderboard_svc
```  
  
Payment Service 
```shell
docker pull pknadimp/payment_svc
docker run -d -p 6000:6000 pknadimp/payment_svc
```

Streak Service
```shell
docker pull pknadimp/streak_svc
docker run -d -p 5000:5000 pknadimp/streak_svc
```

### User Interface

```shell
npm install --save-dev rollup
npm run deploy
```
