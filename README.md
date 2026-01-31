# IT23764798

This project is an automation framework built using Playwright and TypeScript to validate Singlish-to-Sinhala translations on the Swift Translator website.

Key Features:-
Human-like Typing: Uses delayed typing (150ms) to correctly trigger real-time translations.
Smart Waiting Logic: Detects Sinhala output using Unicode regex ([\u0D80-\u0DFF]) to avoid capturing incomplete results.
Data-Driven Testing: Test cases are managed through an external testData.json file for easy scalability.

Technologies Used:-
Playwright
TypeScript

Project Structure:-
tests/singlish_test.spec.ts – Main automation script
testData.json – Test case data
playwright.config.ts – Configuration for headed mode, screenshots, and tracing

How to Run:-
Run tests: npx playwright test --project=chromium
View report: npx playwright show-report
