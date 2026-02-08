### “What trade-offs would you revisit if you did this again?”

“If I were to revisit the design, I would re-evaluate our web server choice earlier. We retained Apache HTTPD due to timelines, but with more planning time, moving to a more cloud-native option upfront could have simplified state management and reduced late-stage risk.”  

### “How did you ensure customer-facing impact was minimal?”

“We followed an incremental migration strategy. Customer-facing workflows were identified early, backward compatibility was maintained, and we validated behavior through load and failover testing before go-live. We also had rollback mechanisms in place to quickly recover if needed.”  

### “How did you measure success?”

“We measured success across three dimensions — system stability, scalability, and productivity. Post-migration, we saw reduced downtime, improved response times during peak traffic, and significantly faster environment setup for development and testing teams.”  

### “What failed during migration?”

“One issue we encountered late was session persistence under high load. Our POC didn’t fully expose this, and it surfaced during scalability testing. We addressed it by introducing Redis-based session management, which stabilized authentication flows without delaying the release.”  

### “What would you change if you had more time?”

“With more time, I would invest more in early performance testing and further standardize components to make the platform even more cloud-native. This would reduce operational complexity and make future scaling easier.”  

### “How did you balance speed vs correctness?”

“We balanced speed and correctness by prioritizing correctness for customer-facing flows while allowing controlled flexibility for internal components. Wherever possible, we chose incremental improvements over large disruptive changes to avoid introducing instability.”  

### “How did you convince stakeholders to accept the hybrid model?”

“I framed the hybrid model as a risk-reduction strategy rather than a compromise. By clearly explaining the constraints around CMS tooling and showing how the hybrid approach would still meet scalability and reliability goals, stakeholders aligned with the decision.”

### “What metrics told you this migration was successful?”

“The key metrics were reduced downtime during peak events, improved page load times, faster environment provisioning, and fewer environment-related production issues. These collectively showed improved reliability and operational efficiency.”
