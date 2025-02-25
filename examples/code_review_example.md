# Code Review Assistant

## Metadata
- **Created**: 2024-02-25
- **Model**: GPT-4
- **Category**: Coding
- **Tags**: code review, best practices, Java, Spring Boot

## Prompt
```
You are a senior Java developer with expertise in Spring Boot applications. I want you to review the following Java code and provide constructive feedback based on:

1. Code quality and readability
2. Spring Boot best practices
3. Potential bugs or security issues
4. Performance considerations
5. Suggestions for improvement

Please organize your feedback into these categories and explain your reasoning for each point. For any issues you identify, provide a specific code example showing how to fix it.

Here is the code to review:

```java
[PASTE CODE HERE]
```
```

## Purpose
This prompt helps developers get professional code reviews for their Java/Spring Boot code. It asks the LLM to analyze code from multiple perspectives and provide actionable feedback with specific examples.

## Example Usage
Use this prompt when you've written a piece of Java/Spring Boot code and want feedback before submitting it for review. Replace the `[PASTE CODE HERE]` section with your actual code.

## Sample Response
```
# Code Review Feedback

## Code Quality and Readability
- The method `processUserData()` is too long (42 lines). Consider breaking it down into smaller, focused methods.
- Variable names like `x` and `temp` are not descriptive. Consider more meaningful names.
- Inconsistent indentation in the `for` loop at line 27.

Suggested improvement for the method length:

```java
public void processUserData(User user) {
    validateUserInput(user);
    transformUserData(user);
    saveUserToDatabase(user);
}

private void validateUserInput(User user) {
    // validation logic here
}

private void transformUserData(User user) {
    // transformation logic here
}

private void saveUserToDatabase(User user) {
    // saving logic here
}
```

## Spring Boot Best Practices
- Using field injection with `@Autowired` is not recommended. Use constructor injection instead.

Current code:
```java
@Service
public class UserService {
    @Autowired
    private UserRepository userRepository;
    
    // methods...
}
```

Improved version:
```java
@Service
public class UserService {
    private final UserRepository userRepository;
    
    public UserService(UserRepository userRepository) {
        this.userRepository = userRepository;
    }
    
    // methods...
}
```

... [additional sections would continue]
```

## Notes
This prompt works best when you provide complete classes or methods rather than snippets without context. For large codebases, consider reviewing one class at a time.
