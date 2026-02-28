```markdown
# AGENTS.md - Guidelines for AI Coding Agents

These guidelines are designed to ensure consistent, maintainable, and high-quality code for our AI coding agents.  Adherence to these principles will maximize productivity and minimize unnecessary complexity.

## 1. DRY (Don't Repeat Yourself)

*   **Single Responsibility Principle:** Each agent should have a single, clearly defined purpose.  Avoid creating agents with overly broad functionalities.
*   **Abstraction:**  Design agents to abstract away implementation details.  Minimize reliance on specific, redundant code.
*   **Code Reuse:**  Strive to create reusable components and patterns.  Utilize existing libraries and frameworks whenever possible.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimalism:**  Code should be concise and easy to understand. Avoid unnecessary complexity.
*   **Readability:**  Prioritize code that is easily readable and understandable. Use clear variable names and consistent formatting.
*   **Efficiency:**  Focus on providing a functional solution, not necessarily the absolute most efficient.

## 3. SOLID Principles

*   **Single Responsibility:** As stated above, each component must have a single purpose.
*   **Open/Closed Principle:**  The agent’s design should allow extensions without modifying existing functionality. (This is primarily applicable to API design)
*   **Liskov Substitution Principle:**  Subclasses should be able to replace parent classes without breaking the system’s behavior. (Primarily applicable to agent logic)
*   **Interface Segregation Principle:**  Clients should not be forced to depend on methods they do not use. (Focus on well-defined interfaces)

## 4. YAGNI (You Aren't Gonna Need It)

*   **Future-Proofing:**  Avoid adding functionality that is unlikely to be required in the future.
*   **Core Functionality:**  Ensure that agents maintain their core functionality without introducing unnecessary complexity.

## 5. Development Process

*   **Code Reviews:** All code must be reviewed by at least one other member of the team before merging.
*   **Unit Testing:**  All agents must have comprehensive unit tests covering all core functionality.  Tests should pass with 90% confidence.
*   **Integration Testing:**  Steps to test the interaction between multiple agents.
*   **Regression Testing:**  Automated tests to verify that changes don’t break existing functionality.  Maintain a robust regression test suite.
*   **Version Control:** Use Git for version control, with proper branching and pull requests.
*   **Documentation:**  Clear and concise documentation for each agent is mandatory.  Document input parameters, output values, and error handling.

## 6. Code Size & Line Limits

*   **Maximum Code Length:**  180 lines of code per agent.
*   **Code Splitting (Conceptual):**  Break down larger agents into smaller, more manageable components for better performance.

## 7. Testing

*   **Test Coverage:**  Aim for at least 80% test coverage.  Use automated testing frameworks.
*   **Test Case Design:** Each test case must cover a specific aspect of the agent’s behavior.
*   **Test Data Management:** Use realistic test data to ensure the agent behaves correctly under various scenarios.
*   **Mocking:** *Only* use mocks during testing.  Do not use real implementation details.

## 8. File Structure & Best Practices

*   **Modular Design:**  Break down the agent into independent modules with clear interfaces.
*   **Naming Conventions:**  Use consistent and descriptive naming conventions (e.g., camelCase, snake_case).
*   **Comments:**  Add clear and concise comments to explain complex logic.
*   **Error Handling:**  Implement robust error handling and logging.

## 9.  Specific Considerations (Example – Adapt as Needed)

*   **Agent A:**  `AgentA.py`:  Handles simple data retrieval.  Requires a unit test.
*   **Agent B:**  `AgentB.py`:  Implements a more complex logic algorithm.  Requires integration tests.
*   **Agent C:**  `AgentC.py`:  Acts as a gateway for other agents.  Requires API interaction tests.

## 10.  Future Considerations (Not Mandatory, but Encouraged)

*   **Monitoring:** Implement basic monitoring to track agent performance.
*   **Configuration Management:**  Introduce a mechanism for managing agent configurations.
*   **API Versioning:** Consider API versioning for greater flexibility.

These guidelines are a living document and will be updated as the project evolves.  Any changes must be thoroughly discussed and approved by the team.  Let's strive for a consistent, high-quality codebase.
```