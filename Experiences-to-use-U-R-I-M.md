## “If PayPal asked you to migrate a critical payment-adjacent system to the cloud today, what principles from this experience would you apply first?”

Cover
- Principles first → execution later
- Risk isolation
- Validation before commitment
- Customer impact awareness

> [!Important]
>
> Mental framework you can reuse (remember this)
> Whenever you get a system design or migration question, think:
>
> **U-R-I-M**
>
> - Understand workflows & users
> - Risk isolation & constraints
> - Incremental validation (POC, testing)
> - Minimize customer impact

“Based on my previous migration experience, I’d start with a few core principles rather than jumping straight into infrastructure decisions.

First, I’d **deeply understand the existing system** — its critical workflows, data dependencies, and traffic patterns — especially which parts are customer-facing and most sensitive to failure.

Second, I’d **assess cloud readiness.** I’d identify which components can be lifted as-is, which need refactoring to become stateless or cloud-friendly, and which might need to remain isolated initially to reduce risk.

Third, I’d **favor an incremental migration approach.** I’d validate assumptions through a proof of concept and targeted stress testing to expose scalability, state management, and data consistency risks early, before full rollout.

Infrastructure sizing and auto-scaling decisions would be driven by observed traffic patterns and test results, not assumptions.

Throughout the process, I’d prioritize **minimizing customer impact** — using techniques like backward compatibility, gradual traffic shifting, and rollback strategies — so migration improves reliability rather than introducing instability.”  

## “Tell me about a time you had to push back on stakeholders to protect system stability or customer impact.”

