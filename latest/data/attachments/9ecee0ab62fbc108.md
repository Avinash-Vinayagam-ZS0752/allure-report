# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: login/system-rejects-login-attempt-with-both-invalid-email-and-password.spec.ts >> System Rejects Login Attempt with Both Invalid Email and Password
- Location: tests/login/system-rejects-login-attempt-with-both-invalid-email-and-password.spec.ts:7:5

# Error details

```
Test timeout of 180000ms exceeded.
```

```
Error: locator.click: Test timeout of 180000ms exceeded.
Call log:
  - waiting for locator('#dummy')

```

# Page snapshot

```yaml
- generic [active]:
  - main:
    - generic [ref=e3]:
      - generic [ref=e5] [cursor=pointer]: 
      - generic [ref=e6]:
        - generic [ref=e7]:
          - generic [ref=e8]:
            - generic [ref=e9]: Privacy Policy
            - generic [ref=e10]: updated January,2022
          - generic [ref=e11]: At Congruent, we recognise the importance of privacy. Our privacy policy applies to all of the products and services offered by Congruent. This privacy policy sets out how Congruent uses and protects any data that you give, when you use this website. Congruent is committed to ensuring that your privacy is protected. When we ask you to provide certain information, by which you can be identified while using this website, you can rest assured that it will only be used in accordance with this privacy statement.
        - img [ref=e13]
      - generic [ref=e15]:
        - generic [ref=e16]:
          - generic [ref=e17]: Changes to this policy
          - generic [ref=e18]: Please note that this privacy policy may change from time to time, so we encourage you to review this policy periodically. The changes will be minor and will continue to protect your rights. Each version of this policy will be identified at the top of the page by its effective date, and we will also keep prior versions of this privacy policy, in an archive, for your review.If you have any questions about this privacy statement or this website, you can write to info@cspl.com or at Privacy Matters, c/o Congruent Solutions, Inc., 19925 Stevens Creek Blvd, Cupertino, CA 95014 USA.
        - generic [ref=e19]:
          - generic [ref=e20]: Collection and usage of information
          - list [ref=e22]:
            - listitem [ref=e23]: In general, a visitor using our website will be anonymous. We do not engage in any activity that will personally identify the visitors to our website.
            - listitem [ref=e24]: Should you need any business information from Congruent, please provide us consent to use your ‘Personal data’ such as your name, e-mail address and phone number, to enable us to contact you for business purposes only. At any point in time, you may choose to revoke/modify/object to your consent to use the personal data, by sending an e-mail to info@cspl.com. Your request will be addressed within 30 calendar days.
            - listitem [ref=e25]: We use your IP address to understand the broad demographic information of the user.
        - generic [ref=e26]:
          - generic [ref=e27]: Controlling your personal information
          - generic [ref=e28]: Using congruentsolutions.com does not require registration of any kind, other than voluntary registration for white papers. The personal data collected will not be shared with, or sold to, anyone outside the company, and will be solely used within Congruent for one-on-one contact with the registrants. Any information that we have collected or stored about you, will be used only in line with the consent you have provided. The data collected is stored by Congruent in a secure server. You may rest assured that we will not give or sell the information to anyone.
        - generic [ref=e29]:
          - generic [ref=e30]: Security
          - generic [ref=e31]: We are committed to ensuring that your information is secure. In order to prevent unauthorised access or disclosure, we have put in place suitable physical, electronic, and managerial measures to safeguard and secure the information we collect online.
        - generic [ref=e32]:
          - generic [ref=e33]: Use of cookies
          - generic [ref=e34]: A cookie is a small file that will be placed on your hard drive. We use cookies to identify the pages being used. Cookies allow web applications to respond to you as an individual. The web application can tailor its operations to your needs, likes and dislikes, by gathering and remembering information about your preferences. This, in turn, helps us analyze data about web page traffic and improve our website. We use this information purely for statistical analysis purposes after which, the data is removed from the system. Cookies help us provide you with a better website/browsing experience, by enabling us to monitor the pages you find useful and the ones you do not. A cookie does not, in any way, give us access to your computer or any information about you, other than the data you choose to share with us. You can choose to accept or decline cookies. Should you agree, a file will be added. Most web browsers automatically accept cookies, but you can usually modify your browser setting to decline cookies, if you choose. This may, however, prevent you from taking full advantage of the features of our website.
        - generic [ref=e35]:
          - generic [ref=e36]: Links
          - generic [ref=e37]: This website may contain links to websites other than congruentsolutions.com and coreretirementsolutions.com. Congruent is not responsible for the privacy practices or the contents of such other websites. We do not take any responsibility for the opinions of third parties expressed on our website
        - generic [ref=e38]:
          - generic [ref=e39]: Mailers
          - generic [ref=e40]: Congruent may, if you choose to subscribe, send direct mailers to you at the address given by you. We may also send mailers via e-mail, if you choose to subscribe. You can opt out of these mailers by clicking on the ‘Unsubscribe’ link provided at the bottom of the mailer. We respect your privacy, and, if you choose not to receive such mailers, we will take all steps to remove you from the list.
        - generic [ref=e41]:
          - generic [ref=e42]: Anti spam policy
          - generic [ref=e43]: Congruent recognises the receipt, transmission, or distribution of spam e-mails (unsolicited bulk e-mails) as a major concern, and has taken reasonable measures to minimise the transmission and effect of spam e-mails in its computing environment. All e-mails received by Congruent are subject to spam check, in coordination with our e-mail service provider. Any e-mail identified as spam will be rejected, with sufficient information sent to the Sender for taking necessary action. With this measure, along with other technical spam reduction measures, Congruent hopes to minimise the effect of spam e-mails. Congruent reserves the right to reject and/or report any suspicious spam e-mails, to the authorities concerned, for necessary action, from time to time. Changes to this policy
    - generic [ref=e44]:
      - img [ref=e46]
      - generic [ref=e47]:
        - generic:
          - list
        - generic [ref=e48]:
          - generic [ref=e49]:
            - generic [ref=e50]: Email
            - textbox "Email" [ref=e51]
          - generic [ref=e53]:
            - generic [ref=e54]: Password
            - generic [ref=e55]:
              - textbox [ref=e56]
              - generic [ref=e58] [cursor=pointer]: 
        - generic [ref=e59]:
          - button "Log in" [ref=e60] [cursor=pointer]
          - link "Forgot password?" [ref=e61] [cursor=pointer]:
            - /url: /Identity/Account/ForgotPassword
            - generic [ref=e62]: Forgot password?
    - img "First slide" [ref=e67]
    - generic [ref=e68]:
      - heading "© Congruent Solutions, Inc. All Rights Reserved" [level=1] [ref=e70]
      - heading "Privacy Policy" [level=1] [ref=e73] [cursor=pointer]
      - img "logo" [ref=e76]
```

# Test source

```ts
  1  | import { test, expect } from '@fixtures/index'
  2  | import * as allure from 'allure-js-commons'
  3  | import { LoginPage } from '@pages/login/login.page'
  4  | 
  5  | const BASE_URL = process.env.APP_BASE_URL!
  6  | 
  7  | test(
  8  |   'System Rejects Login Attempt with Both Invalid Email and Password',
  9  |   { tag: ['@regression', '@login'] },
  10 |   async ({ page, observability }) => {
  11 |     await allure.suite('login')
  12 | 
  13 |     const loginPage = new LoginPage(page)
  14 | 
  15 |     try {
  16 |       await test.step('GIVEN - user is on the login page', async () => {
  17 |         await page.goto(BASE_URL)
  18 |         await expect(loginPage.emailInput).toBeVisible()
  19 |       })
  20 | 
  21 |       await test.step('WHEN - user enters an unrecognized email and a random password', async () => {
> 22 |         await page.locator('#dummy').click() // forced failure
     |                                      ^ Error: locator.click: Test timeout of 180000ms exceeded.
  23 |         await loginPage.login('totally.unknown.user@example.com', 'RandomPass456!')
  24 |       })
  25 | 
  26 |       await test.step('THEN - system denies access with a unified invalid login attempt error', async () => {
  27 |         await expect(loginPage.validationSummary).toContainText('Invalid login attempt.')
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