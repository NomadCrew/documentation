# NomadCrew 🌍

[![Go Report Card](https://goreportcard.com/badge/github.com/NomadCrew/nomad-crew-backend)](https://goreportcard.com/report/github.com/NomadCrew/nomad-crew-backend)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

NomadCrew is an open-source group travel coordination platform that combines real-time location sharing, expense tracking, and travel planning into a single, cohesive mobile application.

## Project Vision
Traveling with friends should be about making memories, not managing apps. NomadCrew eliminates the need to switch between multiple applications for group coordination, expense splitting, and location sharing.

## Key Features
- **Real-time Location Sharing**: Keep track of group members with live location updates
- **Expense Management**: Split and track group expenses with ease
- **Group Communication**: Integrated chat and media sharing
- **Trip Planning**: Collaborative travel planning and itinerary management

## Architecture
NomadCrew follows a microservices architecture using modern cloud-native technologies:

- **Backend**: Go (Golang)
- **Frontend**: React Native
- **Database**: PostgreSQL
- **Cache**: Redis
- **Message Queue**: RabbitMQ
- **Infrastructure**: Kubernetes

## Project Structure
```
nomad-crew/
├── backend/
│   ├── user-service/       # User management and authentication
│   ├── trip-service/       # Trip and group management
│   ├── location-service/   # Real-time location tracking
│   ├── chat-service/       # Real-time messaging
│   └── expense-service/    # Expense tracking and splitting
├── mobile/                 # React Native mobile application
├── infrastructure/         # Kubernetes and cloud configuration
└── docs/                   # Documentation and architecture designs
```

## Getting Started

### Prerequisites
- Go 1.21+
- Docker & Docker Compose
- Node.js 18+
- PostgreSQL 15+
- Redis 7+

### Local Development
1. Clone the repository:
```bash
git clone https://github.com/NomadCrew/nomad-crew-backend.git
```

2. Set up environment variables:
```bash
cp .env.example .env
```

3. Start required services:
```bash
docker-compose up -d
```

4. Run the backend:
```bash
cd backend
make run
```

Detailed setup instructions can be found in our [Development Guide](docs/development.md).

## Technical Documentation
- [Architecture Overview](docs/architecture.md)
- [API Documentation](docs/api.md)
- [Development Guidelines](docs/development.md)
- [Deployment Guide](docs/deployment.md)

## Contributing
We welcome contributions! Please read our [Contributing Guidelines](CONTRIBUTING.md) before submitting a pull request.

### Development Process
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Building in Public
This project is being built in public, with regular updates and technical discussions shared on:
- [LinkedIn Development Journey](https://linkedin.com/in/yourusername)
- [Architecture Decision Records](docs/adr)
- [Project Blog](https://dev.to/yourusername)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
Project Lead - [Your Name](https://linkedin.com/in/yourusername)

Project Link: [https://github.com/NomadCrew/nomad-crew-backend](https://github.com/NomadCrew/nomad-crew-backend)

---

Built with ❤️ for travelers who love tech
