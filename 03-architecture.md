# 2. Designing & Proposing Architecture

> Documenting solutions, making architecture decisions with articulated pros/cons, influencing stakeholders to approve a path forward, and ensuring cost/effort is justified.

---

## Evidence

### Assessed legacy system and recommended approach at Entain

**Context:** When I joined Entain, I was asked to assess an ageing public-facing API. The original developers had left, the codebase had large, complex functions, and there were no tests. The business doubted it could be extended. They were also exploring GraphQL and wanted to know whether migration made sense.

**What I did:** Built a proof of concept replicating core functions using GraphQL. Ran performance tests comparing the two approaches. Results showed GraphQL was slower and added complexity without clear benefits for this use case.

Recommended an alternative: systematically refactor the existing API, introduce dependency injection, and add tests to catch regressions. Presented findings and my recommendation to the client.

**Outcome:** The client agreed and formed a team with three additional Mantel developers to complete the work. The refactoring succeeded and the API became maintainable. Client satisfaction led to a contract extension for the TAB NZ migration.

---

### Designed enterprise AI framework at NAB

**Context:** At NAB, I was responsible for designing a self-service AI framework largely on my own. The key stakeholder was often busy, so I needed to make good decisions without much oversight.

**What I did:** Rather than inventing new patterns, I aligned with existing Terraform and Jenkins conventions so other teams could pick it up easily. Modelled the project structure after the AWS AgentCore starter kit. Added integrations with the business's static analysis tools and included standard linting and testing frameworks.

**Outcome:** Created a framework designed for adoption. Other teams can onboard without extensive hand-holding because it follows patterns they already know.

---

### Presented architecture at Wesfarmers

**Context:** The Wesfarmers engagement was a six-week rapid prototype exploring AWS Bedrock AgentCore. I needed to communicate the solution to both technical and business stakeholders.

**What I did:** Designed the end-to-end architecture integrating Slack, Confluence, and SharePoint with the Bedrock-powered chatbot and proposal generation agent. Presented the architecture to stakeholders, explaining how components fit together and the reasoning behind key decisions.

**Outcome:** Stakeholders understood the solution and how it would fit their workflows. The engagement was AWS-sponsored, which reflected confidence in the approach.

![Presenting architecture at Wesfarmers](assets/wesfarmers_presentation.jpg)

---

### Created API documentation at Entain

**Context:** The legacy Entain API had no formal documentation. New consumers struggled to understand how to integrate.

**What I did:** Retrofitted the API with automatically generated OpenAPI specification. This gave consumers a standard, machine-readable format for endpoints, request/response formats, and expected behaviours.

**Outcome:** New consumers could onboard without reverse-engineering the codebase or relying on tribal knowledge.

---

### Completed security review at NAB

**Context:** The NAB AI framework required security approval before proceeding. Enterprise AI workloads have significant security considerations.

**What I did:** Completed a 70+ page AI security review covering data handling, access controls, model governance, and compliance requirements. Worked through the bank's security review process.

**Outcome:** Project received security approval and could proceed. The documentation provides a reference for future AI initiatives.

---

## Summary

Architecture at Lead level isn't just technical design. It's assessing options, making recommendations, gaining buy-in, and enabling teams to execute. The Entain API assessment led to a team forming around my recommendation. The NAB framework was designed for adoption. The Wesfarmers presentation communicated complex decisions to non-technical stakeholders.

---

[← Back to README](README.md) | [Previous: Technical Charter](02-technical-charter.md) | [Next: Enabling Delivery →](04-enabling-delivery.md)
