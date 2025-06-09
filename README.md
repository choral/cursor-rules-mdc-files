# Cursor Rules MDC Files

This repository contains a collection of MDC (Model-Design-Code) files that provide guidelines and best practices for different aspects of web development frameworks. These files serve as reference materials for maintaining consistent coding standards and architectural patterns.

## Project Templates

### project-nextjs-axum.mdc
A comprehensive project template for full-stack applications using Next.js frontend and Axum backend. Includes project structure, development scripts, Docker configuration, CI/CD setup, and environment configuration for a complete development workflow.

### project-nextjs-fastapi.mdc
A project template for full-stack applications combining Next.js frontend with FastAPI backend. Provides project structure, Docker configuration, and essential development setup for building modern web applications.

## Axum Framework Rules

### axum-models.mdc
Guidelines for designing and implementing database models in Axum applications using SQLx or Diesel. Includes best practices for model organization, relationships, query building, error handling, and testing.

### axum-router.mdc
Rules for structuring and organizing routes in Axum applications, including route grouping, middleware implementation, and request handling patterns.

### axum-backend.mdc
Architectural guidelines for building Axum backend applications, covering project structure, dependency management, and core application setup.

### axum-schemas.mdc
Standards for defining and implementing data validation schemas in Axum applications, ensuring type safety and data integrity.

### axum-handlers.mdc
Best practices for implementing request handlers in Axum, including error handling, response formatting, and business logic organization.

## FastAPI Framework Rules

### fastapi-models.mdc
Guidelines for implementing SQLAlchemy models in FastAPI applications, including model structure, relationships, and database interaction patterns.

### fastapi-router.mdc
Standards for organizing and implementing API routes in FastAPI applications, including route grouping and dependency injection.

### fastapi-backend.mdc
Architectural patterns and best practices for structuring FastAPI backend applications, including project organization and core setup.

### fastapi-schemas.mdc
Rules for implementing Pydantic schemas in FastAPI applications, ensuring proper data validation and serialization.

### fastapi-cruds.mdc
Guidelines for implementing CRUD (Create, Read, Update, Delete) operations in FastAPI applications, including best practices for database operations and error handling.

## Usage

These MDC files are designed to be used as reference materials when developing applications with Axum or FastAPI. They provide consistent patterns and best practices to ensure maintainable and scalable codebases.

## Contributing

Feel free to contribute to these guidelines by submitting pull requests or opening issues for discussion.

# Setting Up MDC Files in Your Repository

This section explains how to integrate the MDC files into your existing repository.

## Adding MDC Files to Your Project

1. Add the MDC repository as a remote:
   ```bash
   git remote add mdc <mdc-repository-url>
   ```

2. Fetch the MDC files from the remote repository:
   ```bash
   git fetch mdc
   ```

3. Merge the MDC files into your repository:
   ```bash
   # If you're on the main branch
   git merge mdc/main --allow-unrelated-histories
   
   # If you're on a different branch
   git merge mdc/main --allow-unrelated-histories -m "Merge MDC files from remote repository"
   ```

4. Resolve any merge conflicts if they occur:
   ```bash
   # After resolving conflicts
   git add .
   git commit -m "Resolve merge conflicts with MDC files"
   ```

## Updating MDC Files

To update your MDC files with the latest changes from the remote repository:

```bash
git fetch mdc
git merge mdc/main
```

## Troubleshooting

- If you encounter merge conflicts, resolve them manually by editing the conflicting files
- Make sure to backup your repository before performing any merge operations
- If you need to start over, you can remove the remote and add it again:
  ```bash
  git remote remove mdc
  git remote add mdc <mdc-repository-url>
  ```

