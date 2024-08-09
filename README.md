# Allure-playwright-report

## Allure Playwright Report Setup

### How to Install Allure Playwright Report

1. **Install Allure Playwright and Allure Commandline:**

   ```bash
   npm install -D allure-playwright
   npm install -D allure-commandline

Configure Allure Playwright in Playwright Config: Add allure-playwright to the reporter section of your playwright.config.js or playwright.config.ts file. Here is an example configuration:

module.exports = {
  reporter: [
    ["dot"],
    ["list"],
    ["ortoni-report", reportConfig],
    ["allure-playwright"],
    ["json", { outputFile: "results.json" }]
  ],
  // other configurations
};



3. **Generate and Open Allure Report: After running your tests, generate the Allure report using the following commands:**

```bash
npx allure generate ./allure-results --clean
npx allure open ./allure-report/


4. **Additional Notes:**

```bash
Ensure that you have Java installed on your system, as Allure Commandline requires it.
This setup will enable you to generate beautiful HTML reports using Allure with your Playwright tests. If you need more detailed information, you can refer to the Allure Playwright documentation.

Learn More
Allure Report Documentation
