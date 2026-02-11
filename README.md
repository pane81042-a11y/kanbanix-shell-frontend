# Kanbanix Shell Frontend

Kanbanix Shell is the host application for the Kanbanix microfrontend architecture.

It is responsible for:

- Routing between microfrontends
- Layout structure (sidebar, header, workspace)
- Authentication state management
- Loading remote modules via Module Federation
- Global state initialization
- Shared dependency management

## Architecture

This application uses:

- React
- Webpack Module Federation
- React Router
- Context API / Redux (optional)
- Shared UI library

The shell dynamically loads:

- Board Frontend
- Task Frontend
- Activity Frontend
- Analytics Frontend
- Admin Frontend
- Auth Frontend

## Purpose

The shell ensures microfrontends remain independently deployable while presenting a unified user experience.

## Deployment

Each microfrontend can be deployed independently.
The shell integrates remote entry files at runtime.
