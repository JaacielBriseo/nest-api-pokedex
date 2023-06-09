<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Run on development

1. Clone repository
2. Run

```
yarn install
```

3. Install Nest CLI

```
npm i -g @nestjs/cli
```

4. Set up DB with docker

```
docker-compose up -d
```

5. Clone file **.env.template** and rename it to **.env**

6. Fill env variables on **.env**

7. Run dev server:

```
yarn start:dev
```

8. Seed DB

```
http://localhost:3000/api/v2/seed
```

# Production Build
1. Create file

```
.env.prod
```

2. Fill prod env variables

3. Create docker image
```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```


## Used Stack

- MongoDB
- Nest
