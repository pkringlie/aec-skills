---
name: coi-checker
description: Compare a subcontractor's certificate of insurance (ACORD 25 or similar, as PDF, image, or pasted text) against the insurance minimums in the subcontract or the company's standard requirements, and list every gap with what to ask the sub or their agent to fix. Use this whenever someone uploads or pastes a COI, certificate of insurance, insurance cert, or ACORD form and asks if it is good, complete, compliant, meets the minimums, or what is missing. Trigger even if they only say "check this cert" or "is this sub covered".
---

# COI Checker

Read a certificate of insurance the way a careful project coordinator would: line by line, against a written set of minimums, with a plain list of what is missing. The output is a gap list the user can paste into an email to the sub or their agent.

This skill checks the certificate against the requirements. It does not decide whether the requirements are right, and it is not insurance or legal advice. When something is unusual, say so and point the user to their broker.

## Step 1: Get the minimums

Use the minimums the user gives you (from the subcontract, the prime contract flow-down, or the owner's requirements). If they give none, use the default table below and say that you did.

Default minimums (edit these to match the company's standard subcontract):

| Coverage | Minimum |
|---|---|
| Commercial General Liability, each occurrence | $1,000,000 |
| Commercial General Liability, general aggregate | $2,000,000 |
| Products and completed operations aggregate | $2,000,000 |
| Automobile liability, combined single limit | $1,000,000 |
| Umbrella or excess liability | $5,000,000 |
| Workers compensation | Statutory |
| Employers liability, each accident / disease each employee / disease policy limit | $1,000,000 / $1,000,000 / $1,000,000 |

Default required endorsements and terms (edit as needed):

- Certificate holder is the general contractor, with the correct legal name and address
- Additional insured on CGL for ongoing and completed operations (endorsement listed, not just the box)
- Additional insured on auto liability
- Primary and non-contributory wording on CGL
- Waiver of subrogation on CGL, auto, and workers compensation
- Project or job name in the description of operations
- Carriers rated A- VII or better by A.M. Best

## Step 2: Read the certificate

Pull these fields from the certificate. If a field is blank or unreadable, record it as "not shown" rather than assuming.

- Insured name (the sub) and whether it matches the name on the subcontract
- Certificate holder name and address
- Date issued
- For each policy: carrier, policy number, effective date, expiration date, each limit
- Which boxes are checked for additional insured and waiver of subrogation, and whether endorsement form numbers are listed
- Description of operations text
- Whether the certificate says it is for information only and confers no rights (standard ACORD language, not a gap by itself)

Watch for these common problems, because they are easy to miss:

- An expiration date that has already passed, or that passes before the sub's work is scheduled to finish
- The aggregate limit lower than the per occurrence limit (usually a typo on the cert, still a gap)
- Umbrella shown but with no indication of which underlying policies it sits over
- "Additional insured" box checked but no endorsement form number in the description, which many contracts do not accept
- Certificate holder listed as the owner or a different entity instead of the GC
- A sub-job or different project named in the description of operations
- Workers compensation marked "N/A" or excluded for a sub that has employees on site

## Step 3: Compare and report

Produce the report in this format every time:

```
COI check: [Sub name] for [project or "project not shown"]
Certificate dated [date], expires [earliest expiration date]

Meets minimums
- [Coverage]: [limit shown] (minimum [minimum])

Gaps
1. [Coverage or term]: [what the cert shows] vs [what is required]. Ask for: [specific fix].
2. ...

Needs a closer look
- [Anything unusual, unreadable, or outside what this checklist can judge]

Status: [Accept / Accept with conditions / Do not accept until gaps are closed]
```

How to phrase a gap so it is useful in an email to the agent:

- Name the coverage, state the number on the cert, state the number required, and say exactly what the agent needs to send. "Umbrella shows $2,000,000; subcontract requires $5,000,000. Ask for a revised certificate showing $5,000,000 umbrella or excess, or a written request for an exception."
- For endorsements, ask for the endorsement form itself, not just a new certificate. "Additional insured is checked but no form number is listed. Ask for a copy of the CG 20 10 and CG 20 37 endorsements or the carrier's equivalent."

Status rules:

- Accept: every minimum met, every required term shown, nothing expires before the work ends.
- Accept with conditions: limits are met but a paperwork item is open (a missing endorsement copy, a wrong certificate holder address). Say what the condition is and who clears it.
- Do not accept: a limit is below minimum, a required policy is missing, or a policy is expired.

## Example

Input: an ACORD 25 for "Northside Mechanical LLC" with CGL $1M / $2M, auto $1M, umbrella $2M, workers comp statutory, EL $500K, certificate holder "Main Street Builders", additional insured box checked, no endorsement forms listed, expiration dates all 03/01 next year. User says "check this against our standard subcontract".

Output:

```
COI check: Northside Mechanical LLC for project not shown
Certificate dated 10/02, expires 03/01

Meets minimums
- CGL each occurrence: $1,000,000 (minimum $1,000,000)
- CGL general aggregate: $2,000,000 (minimum $2,000,000)
- Auto liability: $1,000,000 CSL (minimum $1,000,000)
- Workers compensation: statutory

Gaps
1. Umbrella: $2,000,000 shown vs $5,000,000 required. Ask for a revised certificate at $5,000,000 or a written exception request.
2. Employers liability: $500,000 shown vs $1,000,000 required. Ask for a revised certificate at $1,000,000 each.
3. Additional insured: box checked, no endorsement form listed. Ask for copies of the CGL additional insured endorsements for ongoing and completed operations.
4. Waiver of subrogation: not shown on any policy. Ask for the waiver endorsements on CGL, auto, and workers compensation.
5. Description of operations: no project named. Ask for the project name and the GC listed as additional insured in the description.

Needs a closer look
- Policies expire 03/01. If the sub's work runs past that date, calendar a renewal certificate for mid February.

Status: Do not accept until gaps 1 and 2 are closed. Gaps 3 through 5 are paperwork and can be conditions.
```

## Limits of this check

Say this plainly when it matters: the skill reads the certificate, not the policy. A certificate can show a coverage that the policy excludes. For high risk scopes (roofing, demolition, crane work, anything with a residential exclusion question), tell the user to have the broker review the actual endorsements before the sub mobilizes.
