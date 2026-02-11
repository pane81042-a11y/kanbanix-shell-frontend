# Kanbanix Shell Frontend

Kanbanix Shell is the host application in the Kanbanix microfrontend architecture.

It provides the global layout, routing, authentication state, and runtime integration of independently deployed microfrontends.

## Purpose

The shell ensures that all Kanbanix microfrontends operate as a unified application while remaining independently deployable and scalable.

## Responsibilities

- Application routing
- Global layout (sidebar, header, workspace)
- Authentication state handling
- Loading remote microfrontends via Module Federation
- Shared dependency management
- Global error boundaries
- Environment configuration

## Integrated Microfrontends

- Board Frontend
- Task Frontend
- Activity Frontend
- Analytics Frontend
- Admin Frontend
- Auth Frontend

Each microfrontend is deployed independently and dynamically loaded at runtime.

## Tech Stack

- React
- Webpack Module Federation
- React Router
- Context API or Redux
- Axios for API communication

## AWS Always Free Tier Deployment

This application is deployed using a fully serverless architecture:

- Amazon S3 for static hosting
- Amazon CloudFront for CDN distribution
- AWS IAM for deployment permissions
- GitHub Actions for CI/CD
- Route 53 (optional custom domain)

Deployment flow:
1. Code pushed to GitHub
2. GitHub Actions builds the project
3. Build artifacts uploaded to S3
4. CloudFront cache invalidated

## Scalability

- Fully static frontend
- CDN accelerated
- Independent microfrontend deployments
- No server management required

## Portfolio Value

Demonstrates:
- Microfrontend architecture
- Serverless AWS deployment
- Scalable frontend system design
- Enterprise-level modular architecture
