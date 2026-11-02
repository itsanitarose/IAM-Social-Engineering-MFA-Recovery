# IAM: Social Engineering & MFA Recovery

## The Scenario

It's my fourth week on the security team at Northwind Health, and the help desk has escalated an urgent MFA reset request.

Someone claiming to be Dana Whitfield, VP of Finance, says she lost her phone while travelling and needs to register a replacement device.

The caller knows Dana's personal details, but other information doesn't match. Dana's account can also approve payments and access the bank portal.

### 🎫 The Ticket

**Manager's Request**

> "The help desk escalated a call to us. Someone says she's Dana Whitfield, our VP of Finance, locked out while traveling, and wants her MFA reset to a new phone. The agent sounded uneasy, but she gave him everything he asked for. What should have happened, and how do we fix our process?"

## My Approach

At first, this looked like an urgent MFA recovery request. But the caller's suspicious behaviour and conflicting information made me question whether the request was genuine.

I wanted to understand what was really happening, so I started looking into social engineering and how an attacker might manipulate the help desk's recovery process.

From there, I'll assess the warning signs, question whether the information provided really proves identity and suggest safeguards that protect privileged accounts while allowing legitimate employees to regain access.

## What I Noticed

Three details immediately concerned me.

| Area | Finding |
|:-----|:--------|
| **Identity verification** | The caller knew personal details but refused independent verification methods. |
| **Conflicting information** | The UK calling number didn't match the US HR record, and Dana's Austin calendar raised questions about the travel story. |
| **Privileged access** | An unauthorised MFA reset could expose payment approvals and the bank portal. |

My experience in billing and payment support taught me that **verification comes before discussing or changing account information**. If a customer couldn't be verified, I couldn't proceed with their request, regardless of how urgent the situation sounded.

I would apply the same principle here: **no independent verification, no MFA reset**.

## What This Case Study Covers

- Warning signs of voice phishing and impersonation.
- Immediate help desk response and communication.
- Strong and weak identity verification methods.
- A five-step MFA recovery process for privileged accounts.
- Follow-up actions after a suspected impersonation attempt.

## What I Learned

*To be completed after the investigation.*

## Explore the Investigation

| Document | Focus |
|:---------|:------|
| [01. Source Data](01.%20Source%20Data.md) | Original ticket, call notes and account context. |
| [02. Red Flags & Risk Assessment](02.%20Red%20Flags%20%26%20Risk%20Assessment.md) | Warning signs and potential impact. |
| [03. Help Desk Call Handling](03.%20Help%20Desk%20Call%20Handling.md) | Step-by-step call flow, verification and what to say to the caller. |
| [04. Identity Verification Methods](04.%20Identity%20Verification%20Methods.md) | Strong and weak verification options. |
| [05. Privileged Account Recovery](05.%20Privileged%20Account%20Recovery.md) | Five-step recovery process and additional safeguards. |
| [06. Digging Deeper](06.%20Digging%20Deeper.md) | Follow-up actions if the call was an impersonation attempt. |

---

[← Week 3: AI Agent Security Review](https://github.com/itsanitarose/IAM-AI-Agent-Security-Review) · [All Case Studies](https://github.com/itsanitarose/IAM-Case-Studies)

*Northwind Health is fictional. This is a portfolio assessment; no live production systems were changed.*
