# Mikroprojekt
Mikroprojekt is a full-stack web application that lets TPT students rate lessons and their teachers by giving a 1-5 star rating with an optional comment.
## Project tech stack
[![Vue.js](https://img.shields.io/badge/Vue.js-green?logo=vuedotjs&logoColor=white)](https://vuejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-black?logo=express&logoColor=white)](https://expressjs.com/)
[![Prisma](https://img.shields.io/badge/Prisma-blue?logo=prisma&logoColor=white)](https://www.prisma.io/)
[![MySQL](https://img.shields.io/badge/MySQL-blue?logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Bulma](https://img.shields.io/badge/Bulma-turquoise?logo=bulma&logoColor=white)](https://bulma.io/)
[![JavaScript](https://img.shields.io/badge/JavaScript-yellow?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![HTML](https://img.shields.io/badge/HTML-orange?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![Node.js](https://img.shields.io/badge/Node.js-green?logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Vite](https://img.shields.io/badge/Vite-purple?logo=vite&logoColor=white)](https://vitejs.dev/)
## How to setup front-end dev environment
```bash
cd client
```
Install required packages:
```bash
npm i
```
Run localhost server:
```bash
npm run start
```
## How to setup back-end & database dev environment
```bash
cd server
```
Install required packages:
```bash
npm i
```
Open mysql workbench and create a new sql connection. Put the username as **root** and password as **mysql**, make sure you use port **3306**. Inside server directory create a **.env** file and paste there content from **.env.example**. <br>
<br>
Make a new sql file in mysql workbench and create a database:
```bash
CREATE DATABASE mikroprojekt;
```
Push the schema into mysql:
```bash
npx prisma db push
```
Generate prisma client:
```bash
npx prisma generate
```
Seed the database:
```bash
npm run seed
```
Run localhost server:
```bash
npm run start
```
