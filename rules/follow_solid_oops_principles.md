# Cursor Rule: Enforcing SOLID Principles and OOP Best Practices

## Rule Overview
This rule enforces adherence to SOLID principles and object-oriented programming (OOP) concepts throughout the codebase to improve maintainability, extensibility, and testability.

## Detailed Description

### SOLID Principles Implementation

#### Single Responsibility Principle (SRP)
- Each class should have only one reason to change
- Classes should be small, focused, and handle a single concern
- Identify when a class is doing too much (>200-300 lines is a warning sign)
- Extract separate responsibilities into their own classes
- Example: Separate data access, business logic, and presentation logic

#### Open/Closed Principle (OCP)
- Design classes to be extended without modifying existing code
- Use inheritance and interfaces to allow new behavior without changing existing code
- Avoid extensive conditional logic that requires modification for new cases
- Prefer strategy patterns and plugins over direct modification
- Example: Use abstract base classes and extension points rather than modifying existing classes

#### Liskov Substitution Principle (LSP)
- Derived classes must be completely substitutable for their base classes
- Maintain expected behavior when overriding methods
- Do not strengthen preconditions or weaken postconditions in subclasses
- Ensure derived classes respect all contracts of parent classes
- Example: Override methods without changing their fundamental behavior

#### Interface Segregation Principle (ISP)
- Create fine-grained, client-specific interfaces
- Avoid "fat" interfaces that force clients to depend on methods they don't use
- Split large interfaces into smaller, more focused ones
- Example: Define multiple small interfaces rather than a single comprehensive one

#### Dependency Inversion Principle (DIP)
- High-level modules should not depend on low-level modules
- Both should depend on abstractions
- Always inject dependencies rather than instantiating them directly
- Use dependency injection containers when appropriate
- Example: Accept interfaces as constructor parameters rather than concrete implementations

### OOP Concepts Application

#### Encapsulation
- Hide implementation details behind well-defined interfaces
- Use appropriate access modifiers (private, protected, public)
- Validate inputs and maintain invariants within classes
- Provide controlled access to state through methods
- Example: Make fields private and provide public methods to access/modify them

#### Inheritance
- Use inheritance for "is-a" relationships only
- Prefer composition over inheritance for "has-a" relationships
- Document inheritance hierarchies and their intended uses
- Keep inheritance hierarchies shallow (≤3 levels when possible)
- Example: Create specialized subclasses only when they truly represent a type of the parent

#### Polymorphism
- Design for polymorphic behavior through interfaces and abstract classes
- Use method overriding to allow different implementations of the same interface
- Apply the strategy pattern to encapsulate varying behaviors
- Example: Process different types of data through a common interface

#### Abstraction
- Focus on what objects do rather than how they do it
- Hide complex implementation details behind simple interfaces
- Use abstract classes to define partial implementations and contracts
- Example: Create domain-specific abstractions that map to business concepts

## Implementation Guidelines

1. **Code Reviews**: Check for SOLID violations in code reviews
2. **Refactoring**: Identify and refactor existing code that violates these principles
3. **Design Patterns**: Apply appropriate design patterns that support SOLID (Factory, Strategy, Observer, etc.)
4. **Testing**: Write tests that verify the behavior of interfaces rather than implementations
5. **Documentation**: Document the intent and responsibilities of classes and interfaces

## Examples of Violations to Watch For

- God classes that do everything
- Tight coupling between unrelated components
- Conditional logic based on object types
- Duplicated code across inheritance hierarchies
- Direct instantiation of dependencies
- Public fields exposing implementation details

By following this rule, the codebase will become more modular, maintainable, and adaptable to changing requirements.
