# Project Overview

## Project Name

Nomad Crew

## Description

An app designed for creating disposable groups for trips, featuring live location sharing, messaging, media sharing, and expense splitting.

# System Architecture

## 1. Frontend

### Technology

Ionic (VueJS) + Capacitor

### Key Features

- User authentication
- Group creation and management interface
- Live map with location tracking
- Chat functionality
- Media sharing capabilities
- Expense management and splitting tool

### Development Guidelines

- Utilize VueJS's reactivity and Ionic's rich set of UI components for building a seamless user experience across web and mobile platforms.
- Employ Capacitor to integrate native device features like geolocation and camera access in a cross-platform manner.
- Focus on creating a responsive design that ensures a smooth, native-like experience on any device.
- Prioritize security and privacy in features, especially in location sharing and in-app messaging, adhering to best practices.
- Test extensively in a web environment to streamline development before compiling for Android or iOS platforms.

## 2. Backend

### Technology

Go with gRPC for service communication

### Services

- **User Service:** Manages user authentication and profile settings.
- **Group Service:** Handles group creation, joining, and administration.
- **Location Service:** Provides live location tracking and sharing.
- **Messaging Service:** Facilitates in-app messaging and media sharing.
- **Media Service:** Manages uploading and access to shared media content.
- **Expense Service:** Offers expense recording and splitting among group members.

### Development Guidelines

- Implement robust error handling and logging strategies for clarity and maintenance ease.
- Use gRPC for fast, efficient communication between microservices, enhancing performance.
- Adhere to RESTful principles for API design to ensure clarity and standardization.

## 3. Database

### Primary Database

PostgreSQL

### Caching and Real-time Data

Redis

### Schema Design

Initial schema outlines for user profiles, groups, locations, messages, and expenses, incorporating the PostGIS extension for geospatial queries in PostgreSQL.

### Development Guidelines

- Maintain database normalization to ensure data integrity and consistency.
- Apply appropriate indexing, particularly for location data, to improve query performance.

## 4. Messaging and Event Streaming

### Technology

Apache Kafka

### Usage

- Streaming real-time location updates.
- Managing chat and notification services efficiently.

### Development Guidelines

- Configure Kafka topics to segment data streams effectively.
- Ensure system resilience and message persistence through fault-tolerant setups.

## 5. Infrastructure

### Containerization

Docker

### Orchestration

Kubernetes, hosted on Google Cloud Platform (GCP)

### CI/CD

GitHub Actions integrated with JFrog Artifactory for artifact management

### Monitoring and Logging

Prometheus and Grafana for monitoring, Sentry for error tracking

### Storage

MinIO for object storage, particularly for media files

### Development Guidelines

- Create Dockerfiles for containerization, ensuring a consistent environment across development stages.
- Utilize Kubernetes for deploying and managing microservices, focusing on scalability and reliability.
- Establish CI/CD pipelines for automated testing and deployment, enhancing productivity and reliability.
- Implement comprehensive monitoring and alerting with Prometheus and Grafana, alongside real-time error tracking with Sentry.

# Coding Standards and Practices

## Version Control

Utilize Git with GitHub for source code management and collaboration.

## Code Reviews

Mandatory review process for all contributions to the main branch, ensuring code quality and consistency.

## Documentation

Maintain detailed documentation, including inline comments and service-specific README files, for clarity and collaboration.

## Testing

Comprehensive testing strategy, including unit and integration tests, to ensure reliability and functionality.

## Security

Adherence to OWASP security standards, emphasizing the safeguarding of user data and interactions.

# Contribution Guidelines

## Getting Started

Instructions for setting up a local development environment, including necessary tools and configurations.

## Issue Tracking

Clear guidelines for reporting bugs and feature requests, ensuring effective tracking and resolution.

## Pull Requests

Outlined process for submitting changes, including branch naming conventions and review requirements.

## Code of Conduct

Established expectations for respectful and constructive contribution to foster a positive community.

# Project Roadmap

## Phase 1

Initial setup and implementation of core functionalities such as user authentication and group creation.

## Phase 2

Development and integration of advanced features, including real-time location tracking and messaging.

## Phase 3

Expansion to include additional functionalities like media sharing and expense splitting.

## Phase 4

Comprehensive testing across platforms, final optimizations, and deployment.

# Contact and Support

## Maintainers

Contact information for project maintainers for direct support and inquiries.

## Community

Community engagement channels, such as Slack or Discord, for discussion, collaboration, and support.
