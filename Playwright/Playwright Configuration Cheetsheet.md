## Basic Configuration

Here are some of the most common configuration options.



import { defineConfig, devices } from '@playwright/test';

export default defineConfig({

  // Look for test files in the "tests" directory, relative to this configuration file.

  testDir: 'tests',

  // Run all tests in parallel.
  
  fullyParallel: true,

  // Fail the build on CI if you accidentally left test.only in the source code.
  
  forbidOnly: !!process.env.CI,

  // Retry on CI only.
  
  retries: process.env.CI ? 2 : 0,

  // Opt out of parallel tests on CI.
  
  workers: process.env.CI ? 1 : undefined,

  // Reporter to use
  
  reporter: 'html',

  use: {
  
    // Base URL to use in actions like `await page.goto('/')`.
    
    baseURL: 'http://localhost:3000',

    // Collect trace when retrying the failed test.
    
    trace: 'on-first-retry',
  },
  
  // Configure projects for major browsers.
  
  projects: [
  
    {
    
      name: 'chromium',
      
      use: { ...devices['Desktop Chrome'] },
  
    },
 
  ],

  // Run your local dev server before starting the tests.
  
  webServer: {
  
    command: 'npm run start',
    
    url: 'http://localhost:3000',
    
    reuseExistingServer: !process.env.CI,

  },


## Expect Options

import { defineConfig } from '@playwright/test';

export default defineConfig({
 
  expect: {
  
    // Maximum time expect() should wait for the condition to be met.
    
    timeout: 5000,

    toHaveScreenshot: {
    
      // An acceptable amount of pixels that could be different, unset by default.
      
      maxDiffPixels: 10,
    },

    toMatchSnapshot: {
    
      // An acceptable ratio of pixels that are different to the
      
      // total amount of pixels, between 0 and 1.
      
      maxDiffPixelRatio: 0.1,
  
    },
  
  },

}
);

| Option	|Description|
|---------|-----------|
| testConfig.expect	| Web first assertions like expect(locator).toHaveText() have a separate timeout of 5 seconds by default. This is the maximum time the expect() should wait for the condition to be met. Learn more about test and expect timeouts and how to set them for a single test.|
| expect(page).toHaveScreenshot()	| Configuration for the expect(locator).toHaveScreenshot() method.|
| expect(value).toMatchSnapshot()  | Configuration for the expect(locator).toMatchSnapshot() method.|

}
);
