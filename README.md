# GeeCON 2026 Presentation: 10 Billion Records vs. The Regulator: An Architectural Post-Mortem

This repository contains the slides for my presentation delivered at **GeeCON 2026**.

## Description
What happens when your architecture doesn't just fail a performance test, but triggers a national regulatory investigation? In this session, we go inside a critical system failure at a major bank that led to a formal report to BaFin and a complete rethink of our data strategy.
Dealing with 11TB of data on Oracle Exadata taught us that at a certain scale—specifically, the 10-billion-record mark—standard indexing strategies and read-side duplicate checks don't just slow down; they collapse. We will walk through the "War Room" decisions that led us to flip our architecture on its head, moving from ineffective read-side validation to a high-performance write-side integrity strategy.
Key takeaways include:
* The Compliance-Performance Paradox: How to navigate technical decisions when a "bank crash" brings regulators to your door.
* Architectural Pivots: The logic and implementation details of moving validation to the write-side to stabilize massive ingestion pipelines.
* The Great Exit: How we are building a "Zero-Loss" migration strategy to move 10 billion records from legacy Exadata to Cloud PostgreSQL, including the business case that made it possible.

## Content
- 📄 **[10 Billion Records vs. The Regulator.pdf](./10%20Billion%20Records%20vs.%20The%20Regulator.pdf)**: The full slide deck.

## License

This work is licensed under a **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**.

### 🚫 Commercial Use Restriction
The "NonCommercial" (NC) clause of this license means you **cannot** use these materials for commercial purposes without prior written consent. 

**Examples of prohibited commercial use include:**
- Using the slides in a paid training session or workshop.
- Selling the content as part of a book or course.
- Featuring the content on a website that generates revenue through advertisements or paywalls.

### 📩 Requesting Commercial Permission
If you would like to use this presentation for commercial purposes, or if you are unsure if your use case qualifies as commercial, please reach out to me:

- **Email:** martin.ladecky at gmail.com
- **LinkedIn:** https://www.linkedin.com/in/martin-ladeck%C3%BD-9366ba5/

---
