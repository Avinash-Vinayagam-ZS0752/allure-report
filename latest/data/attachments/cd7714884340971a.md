# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: login/system-rejects-login-attempt-with-incorrect-password.spec.ts >> System Rejects Login Attempt with Incorrect Password
- Location: tests/login/system-rejects-login-attempt-with-incorrect-password.spec.ts:8:5

# Error details

```
Error: expect(locator).toContainText(expected) failed

Locator: locator('.validation-summary-errors')
Timeout: 5000ms
- Expected substring  - 1
+ Received string     + 2

- Error in the login process
+ Invalid login attempt.
+

Call log:
  - Expect "toContainText" with timeout 5000ms
  - waiting for locator('.validation-summary-errors')
    11 × locator resolved to <div data-valmsg-summary="true" class="text-danger marg-top-50 validation-summary-errors">…</div>
       - unexpected value "Invalid login attempt.
"

```

```yaml
- list:
  - listitem: Invalid login attempt.
```

# Test source

```ts
  1  | import { test, expect } from '@fixtures/index'
  2  | import * as allure from 'allure-js-commons'
  3  | import { LoginPage } from '@pages/login/login.page'
  4  | 
  5  | const BASE_URL = process.env.APP_BASE_URL!
  6  | const EMAIL = process.env.APP_USERNAME!
  7  | 
  8  | test(
  9  |   'System Rejects Login Attempt with Incorrect Password',
  10 |   { tag: ['@regression', '@login'] },
  11 |   async ({ page, observability }) => {
  12 |     await allure.suite('login')
  13 | 
  14 |     const loginPage = new LoginPage(page)
  15 | 
  16 |     try {
  17 |       await test.step('GIVEN - user is on the login page', async () => {
  18 |         await page.goto(BASE_URL)
  19 |         await expect(loginPage.emailInput).toBeVisible()
  20 |       })
  21 | 
  22 |       await test.step('WHEN - user enters a valid registered email with an incorrect password', async () => {
  23 |         await loginPage.login(EMAIL, 'WrongPassword999!')
  24 |       })
  25 | 
  26 |       await test.step('THEN - system denies access with an invalid login attempt error', async () => {
> 27 |         await expect(loginPage.validationSummary).toContainText('Error in the login process') //Invalid login attempt.
     |                                                   ^ Error: expect(locator).toContainText(expected) failed
  28 |         await expect(page).toHaveURL(/\/Identity\/Account\/Login/)
  29 |       })
  30 |     } finally {
  31 |       await test.step('attach observability artifacts', async () => {
  32 |         await observability.attachArtifacts(test.info())
  33 |       })
  34 |     }
  35 |   }
  36 | )
  37 | 
```