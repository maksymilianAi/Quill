# Existing Copy Examples

Source: Figma designs. Use these as **structural and tonal reference** — not every example is a gold standard. Anti-patterns are flagged explicitly. Style rules in `system_prompt.md` always win over any example below.

---

## Canonical vocabulary

Use these exact terms. Do not paraphrase or invent alternatives.

| Term | Use | Do not use |
|---|---|---|
| HSA | Health Savings Account | "HSA account", "health account" |
| HRA | Health Reimbursement Arrangement | "HRA account" |
| FSA / HCFSA | Flexible Spending Account | "flex account" |
| COBRA | as-is | "COBRA benefits" |
| EOB | Explanation of Benefits | "benefits statement" |
| Reimburse Me | the product feature name | "reimbursement request", "reimburse feature" |
| Pay a Bill | the product feature name | "bill payment", "pay bills" |
| Plan year | the coverage cycle | "benefit year", "annual period" |
| Spend period | the active spending window | "spending window", "spending cycle" |
| Payroll contributions | employer-routed contributions | "salary contributions" |
| Notional accounts | as-is | "virtual accounts" |
| Forfeitures | unused funds returned to employer | "lost funds", "leftover money" |
| Excess contributions | over-limit contributions | "overpayments", "extra money" |
| Excess earnings | interest/gains on excess contributions | "bonus earnings" |
| IRS limit | the statutory contribution cap | "government limit", "max limit" |
| Plan enrollment | signup to a plan | "plan registration" |
| Participant | end user of the benefit | "member", "beneficiary" |
| Benefit card | the physical/virtual payment card | "debit card", "HSA card" |

---

## Anti-patterns — do NOT imitate

These appear in production but violate the style rules. Flag them in audits and propose the corrected version.

| ❌ Anti-pattern | Why it's wrong | ✅ Corrected |
|---|---|---|
| "Effortlessly upload files by simply scanning the QR code with your device's camera." | "Effortlessly" + "simply" = filler | "Scan the QR code with your device's camera to upload files." |
| "Easily track enrollment details, fund movements and related information" | "Easily" = filler; missing Oxford comma | "Track enrollment details, fund movements, and related information." |
| "Great news! Additional accounts have been linked to your login." | "Great news!" = marketing; exclamation mark | "Additional accounts linked to your login." |
| "You're almost there... Finish registration and access your account by simply verifying your email address using the button below" | Ellipsis; "simply" = filler; too long | "Verify your email to finish registration." |
| "Don't Forget to Finish Your Account Verification" | "Don't forget" = padding | "Finish Your Account Verification" |
| "Friendly reminder — you have an uncashed check waiting." | "Friendly reminder" = padding | "You have an uncashed check waiting." |
| "Just a reminder that you have a $[amount] contribution scheduled" | "Just a reminder" = padding | "A contribution of $[amount] is scheduled" |
| "Congratulations on Your Benefits Enrollment Sponsored by [employer Name]!" | Exclamation; too long; mixed caps in `[employer Name]` | "Your Benefits Enrollment Is Confirmed" |
| "Your Statement is Now Available!" | Exclamation mark | "Your Statement Is Now Available" |
| "Congratulations! You Have Met Your [trigger Type]!" | Two exclamations; mixed caps in placeholder | "You've Met Your [Trigger Type]" |
| "Expense Activity Update - Action Required" | Hyphen used as separator; should be em-dash or colon | "Expense Activity Update — Action Required" |
| "Additional accounts added to your login" (email headline) | Sentence case used for email headline — should be Book Style | "Additional Accounts Added to Your Login" |
| "Unfortunately, the payment was unable to be processed" | Passive + filler | "The payment didn't go through" |
| "This may effect your tax filing" | "effect" should be "affect" | "This may affect your tax filing" |

---

## Card descriptions — Reports section

### Invoice Reconciliation
- **Prefund Invoice** — "View prefunding invoice details, including plan enrollments, policy election amounts, and funding calculations."
- **Contribution Invoice** — "Reconcile contribution invoicing and view invoice details. This report is limited to contribution funded accounts."
- **Replenishment Invoice** — "Replenishment invoices fund payments and reimbursements. Reconcile invoices and view details."

### Enrollments
- **Health Plan Enrollment** — "View employee health plan deductible enrollments, coverage details, and HRA status."
- **Participant Account Activity** — "View participant account activity, including claims, contributions, fees, balances, and enrollment details."

### Claims & Funding
- **Claim Activity** — "Track participant claims, including submissions, statuses, payments, and plan year data."
- **Payroll Contributions** — "View payroll contribution details for HSA and notional accounts."
- **End of Year Forfeitures** — ⚠️ current copy is an anti-pattern ("Easily track…"). Preferred: "Track enrollment details, fund movements, and related information."

---

## Modal copy — Request Excess Contribution Withdraw

- **Modal title** — "Request Excess Contribution Withdraw"
- **Modal description** — "Excess contributions are amounts you put into your HSA beyond the IRS annual limit, which must be corrected to avoid taxes and penalties."
- **Excess amount** (field label) — "Amount entered will be debited from your HSA."
- **Excess earnings** (field label) — "Excess earnings include any additional earnings due to the excess contributions, including but not limited to interest or investment earnings. Please consult with your tax advisor for additional assistance."
- **Warning section title** — "Excess contribution correction withdrawal"
- **Warning body** — "By signing this form, I understand that [UMB] will report this distribution to the IRS as an excess contribution. Funds contributed in excess of your contribution limit are subject to penalty and tax unless the excess and earnings are withdrawn by you prior to your tax filing due date, including any extensions, for filing your Federal Income Tax Return."
- **Checkbox** — "I understand the above rules"

---

## Reimbursement flow — Let's Find Your Receipt

- **Page title** — "Let's Find Your Receipt"
- **Body** — "Let's start by adding your documentation. This could be a receipt, bill, or an EOB. We'll be able to pull some details from the document automatically."
- **Contextual link** — "Have a bill you haven't paid yet? Send your payment directly to the provider here – Pay a Bill."
- **Upload area** — "Drag or browse a picture of your receipt"
- **Tooltip (file type error)** — "Please convert the image into an approved file type or ask your provider for an updated receipt as a PDF."
- **Tooltip trigger** — "Receipt not in one of the allowed file types?"
- **QR section title** — "Scan QR Code to Upload File"
- **QR section description** — ⚠️ current copy is an anti-pattern ("Effortlessly upload files by simply scanning…"). Preferred: "Scan the QR code with your device's camera to upload files."

---

## Plan settings — Spend limits (Healthcare FSA)

- **Setting label** — "Ignore point in time election changes"
- **Setting description** — "Most recent election amount will be made available for all dates of coverage"
- **Setting label** — "Spend limits"
- **Tooltip: Total plan limit** — "Limits the total amount that can be spent across the plan within the designated spend period, regardless of individual participants."
- **Tooltip: Person spend limit** — "Limits the amount that can be spent per person within the plan during the designated spend period."
- **Options** — "Total plan limit", "IRS limit", "Person spend limit", "Spend category spend limit"
- **Setting label** — "Spend period"
- **Options** — "Unlimited", "Monthly", "Plan year"

---

## Email copy

### Account & onboarding

- **Benefits enrollment welcome**
  - Headline: ⚠️ anti-pattern — see glossary. Preferred: "Your Benefits Enrollment Is Confirmed"
  - Body: "Take full advantage of your benefits with [Partner Name]. Here you can access your [account names]."
  - Checklist items: "View your account balance and manage expenses.", "Request payments to your provider or reimburse yourself.", "Activate and manage your benefit card.", "Access important notifications about your account.", "Set up payment options for same-day reimbursements."
  - Button: "Register"

- **Account verification reminder**
  - Headline: "Finish Your Account Verification"
  - Body: "You'll need the last 4 digits from the benefit card you received to finish setting up your account."
  - Button: "Register"
  - Fallback: "Button above doesn't work? Try this link:"

- **Complete registration**
  - Headline: "Complete Your Registration"
  - Body: "Verify your email to finish registration and access your account."
  - Button: "Verify"

- **Additional accounts linked**
  - Headline: "Additional Accounts Added to Your Login"
  - Body: "Additional accounts have been linked to your login. Once in your account, you can switch between accounts to view your balance, transactions, and account history."
  - Button: "Log In"

---

### Security & account access

- **Password reset (one-time code)**
  - Headline: "Reset Your Password"
  - Body: "We've received a request to reset your password. If you didn't make this request, ignore this message. Otherwise, set a new password using this one-time code:"

- **Password reset (link)**
  - Headline: "Reset Your Password"
  - Body: "We've received a request to reset your password."
  - Warning block: "Do not share this email with anyone. Customer service representatives will never ask you for this information. Sharing this link allows access to your account, and financial transactions made cannot be recovered."
  - Instructions: "Click the Reset Password button below. The link expires in 1 hour."
  - Button: "Reset Password"

- **Username reminder**
  - Body: "Your username is [username]. If you didn't make this request, contact Customer Support at [service phone number] immediately."

- **Contact info updated**
  - Headline: "Your Contact Information Has Been Updated"
  - Body: "Your {email or phone or address} has been updated {old_value if present} to {new address or phone or email}. If you didn't make this change, contact us immediately."

---

### Contributions & investments

- **Contribution processed**
  - Headline: "Your Contribution Has Processed"
  - Body: "Your contribution of $[amount] processed on [date]. Funds will be available to spend or invest within [hold days] days. Log in to your account for details."
  - Button: "Log In"

- **Upcoming contribution reminder**
  - Headline: "Upcoming Contribution to Your Account"
  - Body: "A $[amount] contribution is scheduled to pull from [payment source] into your HSA on [scheduled date]. Log in to change this or any future scheduled contributions."
  - Button: "Log In"

- **Problem processing contribution**
  - Headline: "Problem Processing Your Contribution"
  - Body: "On [date], we attempted to pull funds for your requested contribution, but the payment didn't go through. To reapply it, create another contribution request with updated banking information."

- **Investment purchase initiated**
  - Headline: "Investment Purchase Initiated"
  - Body: "An investment purchase of $[amount] has been initiated based on your automatic investment settings. Log in to your HSA to view or modify your investment settings."
  - Button: "Log In"

---

### Claims & payments

- **Expense activity — action required**
  - Headline: "Expense Activity Update — Action Required"
  - Body: "Your [Transaction Type] received on [date received] has been updated to a status of [Claim Status]. Log in to view details and available actions to resolve it."
  - Button: "Log In"

- **Expense activity — no action required**
  - Headline: "Expense Activity Update — No Action Required"
  - Body: "Your [Card Swipe/Reimburse Me/Bill Pay] received on [date received] has been updated to a status of [Claim Status]. Log in to view details."
  - Button: "Log In"

- **Claim payment update**
  - Headline: "Update on Your Claim Payment Request"
  - Body: "We've received and approved your claim payment for [approved amount]. This payment has been applied to cover your outstanding balance from a previous unapproved claim requiring repayment. Your current payment request will not be fully issued for this reason. Review your claims history online for details."

- **Action required — payment problem**
  - Headline: "Action Required: Problem Processing Your Payment"
  - Body: "On [date], we attempted to reimburse you through [PayPal/Venmo/Bank Name], but the payment didn't go through. The funds have been returned to their originating account. Log in and confirm your payment details to receive your reimbursement."
  - Button: "Log In"

- **Payment method updated**
  - Headline: "Payment Method Updated"
  - Body: "Your [debit, Venmo, etc.] payment method for reimbursements has been updated. Your changes are saved for future Reimburse Me requests."
  - Button: "Log In"

- **Payment voided**
  - Headline: "Notice: Payment Voided"
  - Body: "We received a request to void your payment to {provider name}. The check has been voided and the money returned to your account. If you didn't make this request, reach out to your provider to confirm your payment status."

- **Check waiting reminder**
  - Headline: "Your Check Is Waiting"
  - Body: "You have an uncashed check waiting. The check was issued to {you/your provider} on {date}. If it isn't cashed by {date}, the check will expire and the money will be returned to your account."
  - Conditional line: "Since the check was sent to your provider, reach out to them to confirm your payment status."

- **Check expired**
  - Headline: "Check Expired: Money Returned to Your Account"
  - Body: "A check for [amount] expired on [date]. The money has been returned to your account. Log in for details."
  - Button: "Log In"

---

### Account status & alerts

- **Card status update**
  - Headline: "Card Is [Active/Locked/Closed/Out for Delivery]"
  - Body: "A card for [cardholder first name] is now [active/locked/closed/out for delivery]. Log in to view details and manage your benefit card."
  - Button: "Log In"

- **New bank account added**
  - Headline: "New Bank Account Added"
  - Verified state: "Your external bank account has been verified and is linked to your <partner name> account. Any pending payments will process automatically. Log in for transaction details."
  - Pending state: "Your external bank account was recently updated, but additional details are needed to verify it. Log in to complete the setup."
  - Failed state: "Your recent attempt to add or update an external bank account didn't verify. Log in to re-enter your bank account details."
  - Button: "Log In"

- **Statement available**
  - Headline: "Your Statement Is Now Available"
  - Body: "Your [frequency] statement is available to view online. Log in to your HSA for account and claim payment details."
  - Button: "Log In"

- **Account deadline alert**
  - Headline: "Account Deadline Alert"
  - Body: "Your plan year is coming to an end. Check your account deadlines so you don't lose any money."
  - Bullet items: "Your <accountname> has <$>."
  - HSA exception: "Your HSA money never expires. There are no deadlines to use your money."
  - Button: "Log In"

- **Account expires soon**
  - Headline: "Your Account Expires Soon"
  - Body: "Your account deadline is approaching. Spend your money so you don't lose it."
  - Bullet items: "Your <accountname> has <$>."
  - HSA exception: "Your HSA money never expires. There are no deadlines to use your money."
  - Footer note: "* Balance as of <current date MM/DD/YYYY>"
  - Button: "Log In"

- **HSA changes due to employment**
  - Headline: "Changes to Your HSA"
  - Body: "We received important changes in your employment status with [Employer name]. This change will result in several impacts to your Health Savings Account (HSA). One of the most important features of an HSA is that it's your account and remains with you even when you change your health plan coverage or leave your current employer. The funds in your HSA are still yours to spend, save, or invest."
  - Section title: "Account Highlights"

- **HSA closure — verification failed**
  - Headline: "Notice of HSA Account Closure"
  - Body: "We were unable to verify your account. Your HSA has been closed. {if returned to employee} Any contributions on the account have been returned to you. This may affect your tax filing; refer to your tax advisor. Log in to view details."
  - Button: "Log In"

- **HSA closure — inactivity**
  - Headline: "Notice of HSA Account Closure"
  - Body: "Due to inactivity with a $0 balance, your HSA has been closed. You can still log in to:"
  - Checklist: "View account history.", "Access tax documentation.", "Download statements."
  - Button: "Log In"

- **Trigger milestone**
  - Headline: "You've Met Your [Trigger Type]"
  - Body: "You've met your [trigger type]. Log in to your account for details on your account or claim payments."
  - Button: "Log In"

---

## Email copy patterns

- Headlines: Book Style Capitalization, subject-verb or noun phrase structure, 4–6 words (up to 8 when carrying required context).
- No exclamation marks in headlines or body.
- Body: 2–3 sentences per paragraph, direct and informative.
- HSA exceptions always called out separately from other account types.
- One CTA button per email, Book Style: "Log In", "Register", "Verify", "Reset Password".
- Sign-off always: "The {partner name} Team".
- Fallback link always: "Button above doesn't work? Try this link:".
- Footer disclaimers use asterisk: "* Balance as of...".
- Bullet/checklist items end with a period.
- Conditional content uses inline labels: "{if returned to employee}", "<only show if provider payment>".

---

## Patterns to follow

- Verb-first in actions: View / Track / Manage / Reconcile / Submit / Review / Scan / Finish.
- Lists use "including": "including claims, contributions, and fees".
- Oxford comma in lists.
- No period unless 2+ sentences.
- Technical terms used as-is: HSA, HRA, notional accounts, forfeitures, COBRA.
- Em-dash (—) for separating clauses; never hyphen (-).
