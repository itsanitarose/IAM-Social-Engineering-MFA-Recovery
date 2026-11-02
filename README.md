# IAM: MFA Recovery & Identity Verification

It's my fourth week on the security team at Northwind Health, and the help desk has escalated an urgent MFA reset request.

Someone claiming to be Dana Whitfield, VP of Finance, says she lost her phone while travelling and needs MFA registered to a replacement device.

The caller provides the correct personal details, but other parts of the call raise concerns. Dana's account can also approve payments and access the bank portal, making an unauthorised reset particularly risky.

*️ *Fictional scenario. Real world analysis.*


## 🎫 The Ticket

**Manager's Request**

> "The help desk escalated a call to us. Someone says she's Dana Whitfield, our VP of Finance, locked out while traveling, and wants her MFA reset to a new phone. The agent sounded uneasy, but she gave him everything he asked for. What should have happened, and how do we fix our process?"

## My Investigation

Five questions guided my investigation:

1. What warning signs should have concerned the help desk agent?
2. What should the agent do during the call, and what should they say to the caller?
3. Which identity verification methods are strong or weak, and why?
4. How should MFA recovery work for privileged accounts?
5. If this was an impersonation attempt, what should happen after the call?

## What I Noticed

Three details immediately concerned me.

| Area | Finding |
|:-----|:--------|
| **Identity verification** | The caller knew personal details but declined further verification and asked the agent not to call back. |
| **Conflicting information** | The UK calling number didn't match HR records, and Dana's Austin meetings raised questions about her travel story. |
| **Privileged access** | An unauthorised MFA reset could expose payment approvals and the bank portal. |

None of these details proves the caller was an impersonator. But together, they make the request too risky to approve without stronger verification.

## My Approach

At first, this looked like an urgent MFA recovery request. But the caller's suspicious behaviour and conflicting information made me question whether the request was genuine.

I wanted to understand what was really happening, so I started looking into social engineering and how an attacker might manipulate the help desk's recovery process.

From there, I assessed the warning signs, questioned whether the information provided really proved identity and developed safeguards that protect privileged accounts while allowing legitimate employees to regain access.

## Top Priority

**No independent identity verification, no MFA reset.**

My experience in billing and payment support taught me that verification comes before discussing or changing account information. If a customer couldn't be verified, I couldn't proceed, regardless of how urgent the request sounded.

I would apply the same principle here. The agent should pause the reset, explain that additional checks are required and use an independently verified  method rather than relying on the details provided during the call.



## Case Study Outcome

My assessment produced:

- An analysis of the warning signs and potential risks.
- A proposed help desk call handling process, including appropriate communication and escalation.
- A comparison of strong and weak identity verification methods.
- A proposed 5 step MFA recovery process for privileged accounts.
- Follow-up recommendations for investigating a suspected impersonation attempt.

These are proposed procedures and controls, not changes implemented in a live environment.

## What I Learned

*To be completed after the investigation and final review.*

## What I'd Improve

*To be completed after the investigation and final review.*


## Explore the Investigation

| Document | Focus |
|:---------|:------|
| [01. Source Data](document/01.Source%20Data.md) | Original call notes and account context. |
| [02. Red Flags & Risk Assessment](document/02.%20Red%20Flags%20%26%20Risk%20Assessment.md) | Warning signs and potential impact. |
| [03. Help Desk Call Handling](document/03.%20Help%20Desk%20Call%20Handling.md) | Call flow, verification checks and what to say to the caller. |
| [04. Identity Verification Methods](document/04.%20Identity%20Verification%20Methods.md) | Strong and weak verification methods. |
| [05. Privileged Account Recovery](document/05.%20Privileged%20Account%20Recovery.md) | Five-step recovery process and additional safeguards. |
| [06. Digging Deeper](document/06.%20Digging%20Deeper.md) | Follow-up actions if the call was an impersonation attempt. |

---

[← Week 3: AI Agent Security Review](https://github.com/itsanitarose/IAM-AI-Agent-Security-Review) · [All Case Studies](https://github.com/itsanitarose/IAM-Case-Studies)


