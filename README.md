# Kanban Board Application - DevOps Project 🚀

## Project Overview
A Kanban Board application built to showcase modern DevOps practices including CI/CD pipelines, Docker containerization, Kubernetes orchestration, and AWS cloud integration.

## Features
- Task Management (CRUD operations, Status management)
- User Authentication (JWT-based security)
- Serverless notifications (AWS Lambda & SES)
- Containerization (Docker)
- Orchestration (Kubernetes)
- Infrastructure Automation (AWS CloudFormation)

## Project Structure
\```
kanban-board-app/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── utils/
│   │   ├── validators/
│   │   └── index.ts
│   ├── .env
│   ├── package.json
│   └── tsconfig.json
├── docker-compose.yml
└── README.md
\```

## Tech Stack
- **Backend**: Node.js, Express, TypeScript
- **Database**: MongoDB
- **Authentication**: JWT & bcryptjs
- **Testing**: Jest & Supertest
- **Containerization**: Docker & Docker Compose
- **Orchestration**: Kubernetes
- **CI/CD**: GitHub Actions
- **Cloud & Serverless**: AWS Lambda, SES, CloudFormation

## Setup Instructions

### Prerequisites
- Node.js v18+
- Docker & Docker Compose
- Git

### Local Development Setup
\```bash
git clone https://github.com/yourusername/kanban-board-devops.git
cd kanban-board-app/backend
npm install
docker-compose up -d
npm run dev
\```

Open `http://localhost:5000` in your browser to verify.

## Environment Variables
\```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/kanban_board
JWT_SECRET=your_secret_key_here
\```

## CI/CD Pipeline
CI/CD workflow configuration is provided in `.github/workflows/`.

## Kubernetes Deployment
Kubernetes manifests located in the `infra/kubernetes/` directory.

## Serverless Notifications
AWS Lambda and SES used for automated email notifications.

## Contributing
Feel free to fork, make changes, and create pull requests.

## License
[MIT](LICENSE)
