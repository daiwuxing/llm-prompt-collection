# Technical Documentation Generator

## Metadata
- **Created**: 2024-02-25
- **Model**: Claude 3
- **Category**: Writing, Technical Documentation
- **Tags**: documentation, technical writing, API docs, developer guides

## Prompt
```
You are an expert technical writer specializing in creating clear, concise, and comprehensive documentation for software developers.

I need you to create [DOCUMENT_TYPE] documentation for a [TECHNOLOGY_TYPE] [PROJECT_TYPE] called [PROJECT_NAME]. 

The target audience is [AUDIENCE_TYPE] developers with [EXPERIENCE_LEVEL] experience in this technology.

The documentation should follow these guidelines:
- Use clear, concise language appropriate for the target audience
- Include relevant code examples where helpful
- Organize content logically with proper headings and structure
- Explain complex concepts clearly without unnecessary jargon
- Include diagrams or visual aids where appropriate (described in text)
- Follow industry best practices for technical documentation

Here's the information about the project:
[PROJECT_DESCRIPTION]
[KEY_FEATURES]
[TECHNICAL_DETAILS]

Please structure the documentation as follows:
1. Introduction/Overview
2. Getting Started (prerequisites, installation, basic usage)
3. Core Concepts
4. [ADDITIONAL_SECTIONS]
5. API Reference (if applicable)
6. Troubleshooting/FAQ
7. Examples

For code examples, please use syntax highlighting and provide explanatory comments.
```

## Purpose
This prompt helps generate professional technical documentation for software projects, APIs, libraries, or other technical products. It produces well-structured documentation targeted to specific developer audiences.

## Example Usage
Replace the placeholders:
- `[DOCUMENT_TYPE]`: "user guide", "API reference", "developer documentation", etc.
- `[TECHNOLOGY_TYPE]`: "Java", "Spring Boot", "REST", "GraphQL", etc.
- `[PROJECT_TYPE]`: "API", "microservice", "library", "framework", etc.
- `[PROJECT_NAME]`: The name of your project
- `[AUDIENCE_TYPE]`: "backend", "frontend", "full-stack", "DevOps", etc.
- `[EXPERIENCE_LEVEL]`: "beginner", "intermediate", "advanced", etc.
- `[PROJECT_DESCRIPTION]`: Brief overview of what the project does
- `[KEY_FEATURES]`: List of main features or capabilities
- `[TECHNICAL_DETAILS]`: Important technical aspects (technologies used, architecture, etc.)
- `[ADDITIONAL_SECTIONS]`: Any specific sections needed for your project

Example:
```
You are an expert technical writer specializing in creating clear, concise, and comprehensive documentation for software developers.

I need you to create user guide documentation for a Java Spring Boot microservice called CustomerProfileService. 

The target audience is backend developers with intermediate experience in this technology.

The documentation should follow these guidelines:
- Use clear, concise language appropriate for the target audience
- Include relevant code examples where helpful
- Organize content logically with proper headings and structure
- Explain complex concepts clearly without unnecessary jargon
- Include diagrams or visual aids where appropriate (described in text)
- Follow industry best practices for technical documentation

Here's the information about the project:
The CustomerProfileService is a RESTful microservice that manages customer profile data for an e-commerce platform. It handles customer information, preferences, purchase history, and account settings.

Key features:
- CRUD operations for customer profiles
- Authentication and authorization
- Data validation and sanitization
- Integration with order and payment services
- Caching and performance optimizations
- Audit logging and compliance features

Technical details:
- Java 17 with Spring Boot 3.1
- Spring Data JPA with PostgreSQL
- Spring Security with JWT authentication
- Redis for caching
- RabbitMQ for event messaging
- Deployed as Docker containers on Kubernetes

Please structure the documentation as follows:
1. Introduction/Overview
2. Getting Started (prerequisites, installation, basic usage)
3. Core Concepts
4. Authentication and Security
5. Integration with Other Services
6. Performance Considerations
7. API Reference
8. Troubleshooting/FAQ
9. Examples

For code examples, please use syntax highlighting and provide explanatory comments.
```

## Sample Response
(The response would include a complete technical documentation document with all the requested sections)

## Notes
- Adjust the structure based on the type of documentation needed
- For API documentation, consider adding more specific requirements about endpoint documentation format
- For large projects, you might want to break this into multiple prompts for different documentation sections