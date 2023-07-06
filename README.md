# TypeScript Style Guide

[![GitHub](https://srv-cdn.himpfen.io/badges/github/github-flat.svg)](https://github.com/sponsors/brandonhimpfen/) &nbsp; [![Buy Me A Coffee](https://srv-cdn.himpfen.io/badges/buymeacoffee/buymeacoffee-flat.svg)](https://www.buymeacoffee.com/brandonhimpfen) &nbsp; [![Ko-Fi](https://srv-cdn.himpfen.io/badges/kofi/kofi-flat.svg)](https://ko-fi.com/brandonhimpfen) &nbsp; [![PayPal](https://srv-cdn.himpfen.io/badges/paypal/paypal-flat.svg)](https://paypal.me/brandonhimpfen) &nbsp; [![Sponsor Project](https://srv-cdn.himpfen.io/badges/sponsor-project/sponsor-project-flat.svg)](https://brandon.tiny.us/donate)

This guide provides a set of guidelines and best practices for writing TypeScript code. Adhering to these standards will improve code readability, maintainability, and collaboration within your project.

## Table of Contents

1. [General Guidelines](#general-guidelines)
2. [Naming Conventions](#naming-conventions)
3. [Types](#types)
4. [Interfaces](#interfaces)
5. [Classes](#classes)
6. [Functions](#functions)
7. [Variables](#variables)
8. [Modules](#modules)
9. [Error Handling](#error-handling)
10. [Formatting](#formatting)

## General Guidelines

- Always use strict mode by enabling the `strict` compiler option.
- Use meaningful and descriptive names for variables, functions, classes, etc.
- Keep lines of code short and concise. Aim for a maximum of 80 characters per line.
- Comment your code to explain complex logic or any non-obvious behavior.

## Naming Conventions

- Use camelCase for variables, functions, and class members.
- Use PascalCase for classes, interfaces, and type names.
- Use uppercase snake case for constants and enum values.
- Prefix interfaces with `I`.
- Use clear and descriptive names, even if it results in longer names.

## Types

- Prefer TypeScript's built-in types (`string`, `number`, `boolean`, etc.) over their JavaScript counterparts (`String`, `Number`, `Boolean`, etc.).
- Use union types (`|`) and intersection types (`&`) when appropriate.
- Avoid using the `any` type whenever possible. Instead, be explicit about the types.
- Use type inference when the type is obvious and doesn't harm readability.

## Interfaces

- Define interfaces for objects or classes that share a common structure.
- Name interfaces using PascalCase.
- Use optional properties (`?`) or default values sparingly.
- Prefer readonly properties where applicable.

## Classes

- Use classes to represent complex data structures or encapsulate behavior.
- Use the `public` modifier explicitly for clarity, as it's the default access modifier.
- Keep the number of properties and methods in a class to a minimum for better cohesion.
- Prefer composition over inheritance, unless there's a strong need for inheritance.

## Functions

- Use arrow functions (`() => {}`) for short, concise functions and when lexical scoping is required.
- Use regular functions (`function () {}`) for methods and when dynamic scoping is needed.
- Prefer explicit return types for functions to enhance readability.
- Use default parameters to provide optional arguments when it makes sense.

## Variables

- Use `const` for values that should not be reassigned.
- Use `let` for variables that can be reassigned.
- Avoid using `var` unless you have a specific reason to use it.

## Modules

- Use ES modules (`import`/`export`) for managing dependencies.
- Prefer named exports over default exports to encourage explicit imports.
- Organize imports in alphabetical order and group them by third-party dependencies and local modules.

## Error Handling

- Use proper error handling techniques, such as `try-catch` blocks, for handling expected errors.
- Throw specific error types instead of generic `Error` objects.
- Avoid swallowing errors by using empty `catch` blocks.

## Formatting

- Use two spaces for indentation. Do not use tabs.
- Use single quotes (`'`) for string literals, unless escaping is necessary.
- Use semicolons at the end of each statement.
- Put spaces around operators (`+, -, *, /, =, ===, etc.`) for improved readability.
- Break long statements or expressions into multiple lines for better readability.
