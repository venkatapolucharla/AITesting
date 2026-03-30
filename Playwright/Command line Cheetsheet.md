## Basic Playwright Commands
These commands cover the basics of creating a Playwright project, running tests, and generating code. Remember to run these commands in your project directory after initializing your Playwright project.

# Create a New Playwright Project
   
npm init playwright@latest

#. Run Tests

npx playwright test

# Run Tests in UI Mode

npx playwright test --ui

# Run Tests in a Specific Browser

npx playwright test --project=chromium

# Generate Code

npx playwright codegen

# Show Playwright Report

npx playwright show-report

## Debugging Playwright Tests
The Playwright Inspector allows you to step through your tests, inspect the DOM, and interact with the page.

# Using the Playwright Inspector
# Run tests with the inspector

npx playwright test --debug

# Run a specific test file with the inspector

npx playwright test example.spec.ts --debug













