<p align="center">
  <img src="./assets/logo.svg" width="100" />
</p>
<h1 align="center">Chronos</h1>
<p align="center">
    <em>Calendar application Nest API</em>
</p>
<p align="center">
  <a href="https://chronos.mkloz.com">🌐 Website</a> |
  <a href="https://api.mkloz.com/chronos/api/docs">🛠️ API Docs</a> |
  <a href="https://github.com/mkloz/chronos-frontend">💻 Frontend Code</a>
</p>
<p align="center">
 <img src="https://img.shields.io/github/license/maxkrv/chronos-be?style=flat&color=0080ff" alt="license">
 <img src="https://img.shields.io/github/last-commit/maxkrv/chronos-be?style=flat&logo=git&logoColor=white&color=0080ff" alt="last-commit">
 <img src="https://img.shields.io/github/languages/top/maxkrv/chronos-be?style=flat&color=0080ff" alt="repo-top-language">
 <img src="https://img.shields.io/github/languages/count/maxkrv/chronos-be?style=flat&color=0080ff" alt="repo-language-count">
<p>
<p align="center">
  <em>Developed with the software and tools below.</em>
</p>
<p align="center">
 <img src="https://img.shields.io/badge/ESLint-4B32C3.svg?style=flat&logo=ESLint&logoColor=white" alt="ESLint">
 <img src="https://img.shields.io/badge/TypeScript-3178C6.svg?style=flat&logo=TypeScript&logoColor=white" alt="TypeScript">
 <img src="https://img.shields.io/badge/Prisma-2D3748.svg?style=flat&logo=Prisma&logoColor=white" alt="Prisma">
 <img src="https://img.shields.io/badge/Docker-2496ED.svg?style=flat&logo=Docker&logoColor=white" alt="Docker">
    <img src="https://img.shields.io/badge/Node.js-339933.svg?style=flat&logo=Node.js&logoColor=white" alt="Node.js">
    <img src="https://img.shields.io/badge/Zod-000000.svg?style=flat&logo=Zod&logoColor=white" alt="Zod">
    <img src="https://img.shields.io/badge/Prettier-F7B93E.svg?style=flat&logo=Prettier&logoColor=white" alt="Prettier">
    <img src="https://img.shields.io/badge/Swagger-85EA2D.svg?style=flat&logo=Swagger&logoColor=black" alt="Swagger">
    <img src="https://img.shields.io/badge/OpenAPI-6BA539.svg?style=flat&logo=OpenAPI-Initiative&logoColor=white" alt="OpenAPI">
    <img src="https://img.shields.io/badge/Amazon_S3-569A31.svg?style=flat&logo=Amazon-S3&logoColor=white" alt="AWS S3">
    <img src="https://img.shields.io/badge/nestjs-E0234E?style=flat&logo=nestjs&logoColor=white" alt="Nest.js">
    <img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white" alt="PostgreSQL">
    <img src="https://img.shields.io/badge/redis-%23DD0031.svg?style=flat&logo=redis&logoColor=white" alt="Redis">
    <img src="https://img.shields.io/badge/JWT-000000?style=flat&logo=JSON%20web%20tokens&logoColor=white" alt="JWT">
    <img src="https://img.shields.io/badge/axios-671ddf?style=flat&logo=axios&logoColor=white" alt="Axios">

</p>
<hr>

## 🔗 Quick Links

> - [📋 Overview](#-overview)
> - [�� Tech Stack](#-tech-stack)
> - [🗄️ Database Schema](#️-database-schema)
> - [💻 Getting Started](#-getting-started)
>     - [⚙️ Installation](#️-installation)
>     - [🕜 Running Chronos](#-running-chronos)
> - [📜 Swagger Documentation](#-swagger-documentation)
> - [🤝 Contributing](#-contributing)
> - [📄 License](#-license)

---

## 📋 Overview

**Chronos** is a modern, scalable calendar management API built with [Nest.js](https://nestjs.com/) and [TypeScript](https://www.typescriptlang.org/). Designed for teams and individuals, Chronos provides robust tools for managing calendars, scheduling events, sending invitations, and handling user interactions—all with a focus on security and extensibility.

**Key Features:**
- 🗓️ **Calendar Management:** Create, update, and share multiple calendars.
- 📅 **Event Scheduling:** Organize single or recurring events with rich metadata.
- ✉️ **Invitations:** Send and manage event and calendar invitations.
- 👥 **User Roles:** Fine-grained access control for users and guests.
- 🔒 **Secure Authentication:** JWT-based authentication and role-based access.
- ⚡ **Performance:** Caching with Redis and efficient database access via Prisma.
- ☁️ **Cloud Ready:** Dockerized for easy deployment, with AWS S3 integration for file storage.
- 📖 **Interactive API Docs:** Explore and test endpoints via Swagger UI.

> **Repository:** [mkloz/chronos-backend](https://github.com/mkloz/chronos-backend)

---

## 🚀 Tech Stack

- **Core**: [TypeScript](https://www.typescriptlang.org/), [Nest.js](https://nestjs.com/)
- **Database**: [PostgreSQL](https://www.postgresql.org/), [Prisma ORM](https://www.prisma.io/)
- **Caching**: [Redis](https://redis.io/)
- **Authentication**: [JWT](https://jwt.io/), [bcryptjs](https://www.npmjs.com/package/bcryptjs)
- **Storage**: [AWS S3](https://aws.amazon.com/s3/)
- **Email**: [React-email](https://react.email/), [Nodemailer](https://nodemailer.com/)
- **Validation**: [class-validator](https://github.com/typestack/class-validator), [class-transformer](https://github.com/typestack/class-transformer), [zod](https://zod.dev/)
- **HTTP Client**: [axios](https://axios-http.com/)
- **Security**: [helmet](https://helmetjs.github.io/)
- **Documentation**: [Swagger](https://swagger.io/)
- **Development**: [ESLint](https://eslint.org/), [Prettier](https://prettier.io/), [Husky](https://typicode.github.io/husky/)
- **Containerization**: [Docker](https://www.docker.com/)

---

## 🗄️ Database Schema

The database schema is defined using Prisma. Below is a visual representation of the schema:

<p align="center">
    <img src="prisma/db.jpg" alt="Database Schema" width="600" />
</p>

---

## 💻 Getting Started

### ⚙️ Installation

1. Clone the Chronos repository:

```sh
git clone https://github.com/mkloz/chronos-backend.git
```

2. Change to the project directory:

```sh
cd chronos-backend
```

3. Install the dependencies:

```sh
npm install
```

4. Create a `.env` file in the root directory and add environment variables like in `.env.example` file.

### 🕜 Running Chronos

Use the following command to run the Chronos application:

```sh
npm run dev
```

---

## 📜 Swagger Documentation

To view the Swagger documentation for the Chronos API, follow these steps:

1. Ensure the Chronos application is running.
2. Open your web browser and navigate to `http://localhost:6969/api/docs#/`.

This will open the Swagger UI, where you can explore and test the API endpoints interactively.

--

---

## 🤝 Contributing

Contributions are welcome! Here are several ways you can contribute:

- **[Submit Pull Requests](https://github.com/mkloz/chronos-backend/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
- **[Join the Discussions](https://github.com/mkloz/chronos-backend/discussions)**: Share your insights, provide feedback, or ask questions.
- **[Report Issues](https://github.com/mkloz/chronos-backend/issues)**: Submit bugs found or log feature requests for Chronos-backend.

<details closed>
    <summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your GitHub account.
2. **Clone Locally**: Clone the forked repository to your local machine using a Git client.

    ```sh
    git clone https://github.com/mkloz/chronos-backend
    ```

3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.

    ```sh
    git checkout -b new-feature-x
    ```

4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.

    ```sh
    git commit -m 'Implemented new feature x.'
    ```

6. **Push to GitHub**: Push the changes to your forked repository.

    ```sh
    git push origin new-feature-x
    ```

7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.

Once your PR is reviewed and approved, it will be merged into the main branch.

</details>

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/mkloz/chronos-backend/blob/develop/LICENSE) file for details.
