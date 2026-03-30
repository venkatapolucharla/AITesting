## Basic Playwright Command line commands

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

# Run all tests
npx playwright test

# Run a single test file
npx playwright test tests/todo-page.spec.ts

# Run a set of test files
npx playwright test tests/todo-page/ tests/landing-page/

# Run tests at a specific line
npx playwright test my-spec.ts:42

# Run tests by title
npx playwright test -g "add a todo item"

# Run tests in headed browsers

npx playwright test --headed

# Run tests for a specific project

npx playwright test --project=chromium

# Get help
npx playwright test --help

# Disable parallelization

npx playwright test --workers=1

# Run in debug mode with Playwright Inspector

npx playwright test --debug

# Run tests in interactive UI mode

npx playwright test --ui

Option      	Description
--debug	               Run tests with Playwright Inspector. Shortcut for PWDEBUG=1 environment variable and --timeout=0 --max-                                 failures=1 --   headed --workers=1 options.

--headed	                        Run tests in headed browsers (default: headless).

-g <grep> or --grep <grep>	      Only run tests matching this regular expression (default: ".*").

--project <project-name...>	Only run tests from the specified list of projects, supports '*' wildcard (default: run all projects).

--ui	                        Run tests in interactive UI mode.

-j <workers> or --workers <workers>	   Number of concurrent workers or percentage of logical CPU cores, use 1 to run in a single worker (default: 50%).

## Test list

# This is a test list file.
# It can include comments and empty lines.

# Run ALL tests in a file:
path/to/example.spec.ts

# Run all tests in a file for a specific project:

[chromium] › path/to/example.spec.ts

# Run all tests in a specific group/suite:

path/to/example.spec.ts › suite name

# Run all tests in a nested group:
path/to/example.spec.ts › outer suite › inner suite

# Fully qualified test with a project:

[chromium] › path/to/example.spec.ts:3:9 › suite › nested suite › example test

# This test is included for all projects:

path/to/example.spec.ts:3:9 › example test

# Use "›" or ">" as a separator:

[firefox] > example.spec.ts > suite > nested suite > example test

# Line/column numbers are completely ignored, you can omit them.
# Three entries below refer to the same test:

example.spec.ts › example test

example.spec.ts:15 › example test

example.spec.ts:42:42 › example test

## Show Report

npx playwright show-report [report] [options]

# Show latest test report

npx playwright show-report

# Show a specific report

npx playwright show-report playwright-report/

# Show report on custom port

npx playwright show-report --port 8080

## Install Browsers

npx playwright install [options] [browser...]

npx playwright install-deps [options] [browser...]


npx playwright uninstall

# Install all browsers

npx playwright install

# Install only Chromium

npx playwright install chromium

# Install specific browsers

npx playwright install chromium webkit

# Install browsers with dependencies

npx playwright install --with-deps

## Generation & Debugging Tools
# Code Generation

npx playwright codegen [options] [url]

# Start recording with interactive UI

npx playwright codegen

# Record on specific site

npx playwright codegen https://playwright.dev

# Generate Python code

npx playwright codegen --target=python

## Trace Viewer

Analyze and view test traces for debugging. 

npx playwright show-trace [options] [trace]

# Open trace viewer without a specific trace (can load traces via UI)

npx playwright show-trace

# View a trace file

npx playwright show-trace trace.zip

# View trace from directory

npx playwright show-trace trace/

## Specialized Commands

npx playwright merge-reports [options] <blob dir>

# Combine test reports
npx playwright merge-reports ./reports

# Clear Cache

Clear all Playwright caches.

npx playwright clear-cache






























