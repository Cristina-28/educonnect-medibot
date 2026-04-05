# MediBot — Testing

Testing done in the Copilot Studio Test Chat panel. All interactions are in Romanian.

**Date:** [DATA]

---

## System Topics

**01 — Greeting**
Input: `salut`
Expected: Romanian greeting with bot name
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-01-greeting.png)

**02 — Thank You**
Input: `mulțumesc`
Expected: "Cu plăcere" response
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-02-thankyou.png)

**03 — Escalate**
Input: `vreau să vorbesc cu cineva`
Expected: Message with phone and email
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-03-escalate.png)

**04 — Reset**
Input: `o luăm de la început`
Expected: Asks for confirmation before resetting
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-04-reset.png)

**05 — Fallback**
Input: `asjkdhaskd`
Expected: Asks to rephrase
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-05-fallback.png)

---

## Knowledge Base

**06 — Subjects**
Input: `ce materii aveți?`
Expected: List of EN + BAC subjects
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-06-subjects.png)

**07 — Pricing**
Input: `cât costă matematica pentru BAC?`
Expected: 130 RON (M1) / 120 RON (M2)
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-07-pricing.png)

**08 — Tutor Match**
Input: `ce profesori predau fizică?`
Expected: Vlad Dumitrescu + details
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-08-tutor.png)

**09 — Free Trial**
Input: `aveți ședință de probă?`
Expected: Free, 30 min, one per tutor
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-09-trial.png)

**10 — Payment**
Input: `cum plătesc?`
Expected: Transfer, card, cash (fizic only)
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-10-payment.png)

---

## Edge Cases

**11 — English Input**
Input: `hello`
Expected: Still responds in Romanian
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-11-english.png)

**12 — Cancellation**
Input: `vreau să anulez`
Expected: Cancellation info + 24h policy
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-12-cancel.png)

**13 — Booking**
Input: `vreau să rezerv o ședință`
Expected: Step-by-step: name, class, subject, tutor, format, time
Actual: [RESULT]
Status: ✅ / ❌
![screenshot](screenshots/test-13-booking.png)

---

## Bugs

None yet. Will update as I test.
