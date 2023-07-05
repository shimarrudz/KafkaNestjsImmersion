![Imersão Full Stack && Full Cycle](https://events-fullcycle.s3.amazonaws.com/events-fullcycle/static/site/img/grupo_4417.png)
# KafkaNestjsImmersion
## About the repository

📁 This repository contains the source code taught in the class: Real-Time High Performance: Exploring Nest.js and Kafka [https://www.youtube.com/watch?v=z87Yo6j_iK8](https://www.youtube.com/watch?v=z87Yo6j_iK8)

### Running using docker-compose up:

Go to the `live-imersao-13-nestjs-kafka` folder and open `VSCode`:

```bash
cd live-imersao-13-nestjs-kafka && code .
```

Run the containers with the command:

```bash
docker compose up
```

Enter the `next` container:

```bash
docker compose exec app bash
```

Install the dependencies:

```bash
npm install
```

#### Orders

Run the command for `prisma` to perform the `migrate`:

```bash
cd apps/orders && npx prisma migrate dev
```

To run the application, use the command:

```bash
npm run start:dev
```

#### Payments

Run the command for `prisma` to perform the `migrate`:

```bash
cd apps/payments && npx prisma migrate dev
```

To run the application, use the command:

```bash
npm run start:dev payments
```

NOTE: If you need to stop the containers for any reason, run the command: `docker compose down`, as the `Kafka` container needs to be stopped and restarted.

---

### Dev Container:

Install the dependencies:

```bash
npm install
```

#### Orders

Run the command for `prisma` to perform the `migrate`:

```bash
cd apps/orders && npx prisma migrate dev
```

To run the application, use the command:

```bash
npm run start:dev
```

#### Payments

Run the command for `prisma` to perform the `migrate`:

```bash
cd apps/payments && npx prisma migrate dev
```

To run the application, use the command:

```bash
npm run start:dev payments
```

NOTE: If you need to stop the containers for any reason, follow the steps below:

Press `ctrl + shift + p` and select `Dev Containers: Rebuild Containers`, as the `Kafka` container needs to be stopped and restarted.
