# Java Spring Boot API Development

## Metadata
- **Created**: 2024-02-25
- **Model**: GPT-4
- **Category**: Coding
- **Tags**: java, spring boot, rest api, web development

## Prompt
```
You are an expert Java Spring Boot developer with extensive experience building RESTful APIs. 

I need you to help me implement a [FEATURE_TYPE] for a [BUSINESS_DOMAIN] application using Spring Boot.

Requirements:
- The feature should follow REST best practices
- Use Spring Data JPA for database interactions
- Implement proper exception handling
- Follow clean code principles and SOLID design
- Include unit tests using JUnit 5 and Mockito

Technical constraints:
- Spring Boot version: 3.0+
- Java version: 17
- Database: [DATABASE_TYPE]
- Authentication: [AUTH_METHOD]

[ADDITIONAL_CONTEXT]

Please provide the following:
1. Data model/entity classes
2. Repository interfaces
3. Service layer implementation
4. REST controller
5. Exception handling
6. Unit tests
7. Sample API requests/responses

For each component, explain your design decisions and any best practices you're following.
```

## Purpose
This prompt generates complete, production-ready Spring Boot API components with explanations of design decisions. It's useful for getting up-to-speed on Spring Boot best practices or quickly bootstrapping a new API feature.

## Example Usage
Replace the placeholders:
- `[FEATURE_TYPE]`: "user management system", "product inventory API", etc.
- `[BUSINESS_DOMAIN]`: "e-commerce", "healthcare", "banking", etc.
- `[DATABASE_TYPE]`: "PostgreSQL", "MySQL", "MongoDB", etc.
- `[AUTH_METHOD]`: "JWT", "OAuth2", "Basic Auth", etc.
- `[ADDITIONAL_CONTEXT]`: Add any specific requirements or constraints

Example:
```
You are an expert Java Spring Boot developer with extensive experience building RESTful APIs. 

I need you to help me implement a user management system for an e-commerce application using Spring Boot.

Requirements:
- The feature should follow REST best practices
- Use Spring Data JPA for database interactions
- Implement proper exception handling
- Follow clean code principles and SOLID design
- Include unit tests using JUnit 5 and Mockito

Technical constraints:
- Spring Boot version: 3.0+
- Java version: 17
- Database: PostgreSQL
- Authentication: JWT

Additional context:
- Users should have roles (ADMIN, CUSTOMER, MERCHANT)
- Need endpoints for registration, login, profile management
- Password should be securely stored
- Include email verification flow

Please provide the following:
1. Data model/entity classes
2. Repository interfaces
3. Service layer implementation
4. REST controller
5. Exception handling
6. Unit tests
7. Sample API requests/responses

For each component, explain your design decisions and any best practices you're following.
```

## Sample Response
(The response would include complete code examples with explanations for each component of a Spring Boot API)

## Notes
- This prompt works best with models that have strong coding capabilities like GPT-4
- You can adjust the technical constraints based on your project requirements
- Consider breaking this into smaller prompts for very complex features