# Laravel Movie Database

## About Laravel Movie DB

This is a movie database system built with Laravel for the Software Construction and Evolution course in the Software Engineering Technology Program, Department of Information Technology, Politeknik Negeri Padang.

## Refactoring Changes

The codebase has undergone significant refactoring to improve code quality, maintainability, and security. The following improvements were implemented:

### 1. Consistent URL Generation
- Replaced hardcoded URLs with Laravel's named routes using the `route()` helper
- Added missing route names in the routes file
- Improved maintainability by centralizing route definitions

### 2. Consistent Data Access Patterns
- Standardized model property access using object notation (`$movie->property`) instead of mixing with array notation
- Improved code readability and reduced potential errors

### 3. Enhanced Image Handling
- Implemented the `asset()` helper for all image paths
- Added descriptive alt text for images to improve accessibility
- Centralized image path construction

### 4. Improved Form Structure
- Added validation error display to all forms
- Implemented old input retention to preserve user input on validation errors
- Added consistent form actions and methods
- Added cancel/back buttons for better user experience

### 5. Security Enhancements
- Implemented proper CSRF protection for all forms
- Changed delete operations from GET to POST/DELETE requests
- Added confirmation dialogs for destructive actions

### 6. Code Organization
- Reduced code duplication across views
- Improved naming consistency
- Enhanced readability with proper indentation and spacing

