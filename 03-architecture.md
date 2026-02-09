# 2. Designing & Proposing Architecture

> Documenting solutions, making architecture decisions with articulated pros/cons, influencing stakeholders to approve a path forward, and ensuring cost/effort is justified.

---

## Evidence

### Assessed legacy system and recommended refactoring approach at Entain

**Context:** When I joined Entain, I was tasked with assessing an ageing public-facing API. The original maintainers had left, the codebase was complex with large functions, and there were no tests. The business doubted it could be extended in its current state. They were also building out GraphQL capabilities and wanted to explore whether to migrate.

**What I did:** Produced a proof of concept replicating core functions of the legacy API using GraphQL. Ran performance testing to generate metrics comparing the two approaches. The results showed GraphQL was slower and added cognitive complexity without clear benefits for this use case.

Recommended an alternative approach: systematically refactor the existing API, introduce dependency injection, and add tests to verify we weren't introducing regressions. Presented findings and recommendation to the client.

**Outcome:** Client agreed with the recommendation and formed a team with three additional Mantel developers to complete the project. The refactoring was successful – the API became maintainable and extensible. Client satisfaction led to contract extension for the TAB NZ migration project.

**Leadership demonstrated:** Assessed options, articulated pros/cons, made a recommendation, gained stakeholder buy-in, and enabled a team to execute the agreed approach.

---

### Designed enterprise AI framework with minimal supervision at NAB

**Context:** At NAB, I was responsible for designing a self-service AI framework largely independently. The key stakeholder was often busy and difficult to get time with, so I needed to make good decisions autonomously.

**What I did:** Rather than inventing novel patterns, I aligned with existing Terraform and Jenkins patterns used by the business so my code would be easy for other teams to pick up and understand. Modelled the configuration and project structure after the AWS AgentCore starter kit to leverage familiar conventions.

Took initiative to add integrations with the business's static analysis tools and included industry-standard linting and testing frameworks to ensure quality from the start.

**Outcome:** Created a framework that other teams could adopt without extensive onboarding. The design decisions prioritised maintainability and alignment with existing practices over novelty.

---

### Presented technical architecture to stakeholders at Wesfarmers

**Context:** The Wesfarmers engagement was a six-week rapid prototype exploring AWS Bedrock AgentCore. Needed to communicate the solution architecture to both technical and business stakeholders.

**What I did:** Designed the end-to-end architecture integrating Slack, Confluence, and SharePoint with the Bedrock-powered chatbot and proposal generation agent. Presented the architecture to stakeholders, explaining how the components fit together and the rationale for key decisions.

**Outcome:** Stakeholders understood the solution and how it would fit into their existing workflows. The engagement was AWS-sponsored, reflecting confidence in the approach.

![Presenting architecture at Wesfarmers](assets/wesfarmers_presentation.jpg)

---

### Created API documentation to enable consumer onboarding at Entain

**Context:** The legacy Entain API had no formal documentation. New consumers had difficulty understanding how to integrate.

**What I did:** Retrofitted the API with automatically generated OpenAPI specification documentation. This provided a standard, machine-readable format that consumers could use to understand endpoints, request/response formats, and expected behaviours.

**Outcome:** New consumers could onboard to the integration easily without needing to reverse-engineer the codebase or rely on tribal knowledge.

---

### Completed comprehensive security review at NAB

**Context:** The NAB AI framework project required security approval before proceeding. Enterprise AI workloads have significant security considerations.

**What I did:** Completed a 70+ page AI security review covering data handling, access controls, model governance, and compliance requirements. Worked through the bank's security review process to get the project approved.

**Outcome:** Project received security approval and could proceed. The documentation provided a reference for future AI initiatives.

---

## Summary

Architecture at the Lead level isn't just about technical design – it's about assessing options, making recommendations, gaining buy-in, and enabling teams to execute. My examples demonstrate this full cycle: from the Entain API assessment that led to a team forming around my recommendation, to the NAB framework designed for adoption, to presenting solutions at Wesfarmers.

---

[← Back to README](README.md) | [Previous: Technical Charter](02-technical-charter.md) | [Next: Enabling Delivery →](04-enabling-delivery.md)
