# 3. Enabling Team Delivery

> Ensuring issues/risks are identified with sufficient time, building backlogs with clear acceptance criteria, protecting team focus time, and investing in efficiency improvements.

---

## Evidence

### Led platform strategy and backlog creation (Platform Lead)

**Context:** At Fred, the business deployed infrastructure via ad-hoc click-ops which wasn't scalable. There was no clear platform strategy or roadmap.

**What I did:** Worked with the business to create a strategy for uplifting platform capabilities. Created and prioritised features, got buy-in from stakeholders, and broke features into actionable work items during backlog refinement.

**Outcome:** The team implemented infrastructure-as-code with Terraform, built a release management suite, and set up observability with Datadog and PowerBI. Moved from manual deployments to a repeatable, scalable platform.

---

### Refined backlog into deliverable work at Entain

**Context:** After the Entain API team formed, we had a Product Owner who prioritised features. But business priorities still needed translating into work the developers could pick up.

**What I did:** Worked with the team to refine the backlog into deliverable user stories. Broke down feature areas including observability uplift, performance improvements, OpenAPI documentation, and new API endpoints.

**Outcome:** Developers had clarity on what to build and why. Work was sized appropriately with clear acceptance criteria. The team could focus on delivery rather than constantly seeking clarification.

---

### Built self-service tooling at NAB

**Context:** At NAB, AI initiatives were blocked waiting for the platform team to provision infrastructure and configure deployments. This slowed adoption across the organisation.

**What I did:** Designed a self-service framework so teams could build and deploy Bedrock AgentCore applications independently. Created opinionated templates with schema-validated configuration and automated pipelines that handled the full deployment lifecycle. Aligned with existing Terraform and Jenkins patterns so teams wouldn't need to learn new conventions.

**Outcome:** Teams can now deploy without waiting on the platform team. The investment in tooling reduces friction for every new AI initiative going forward.

---

### Drove quality improvements at Entain

**Context:** The legacy Entain API had no tests. Any change risked introducing regressions, which slowed delivery and reduced confidence.

**What I did:** Championed a quality-first approach during the refactoring. Introduced dependency injection to make the codebase testable. Established testing patterns and worked with the team to build coverage systematically.

**Outcome:** Unit test coverage increased from 0% to 75%. The team could make changes with confidence, which sped up delivery rather than slowing it down.

---

### Set up observability at Entain

**Context:** Without visibility into system behaviour, debugging was time-consuming. Developers couldn't see performance characteristics or trace issues easily.

**What I did:** Set up observability dashboards using Prometheus, Grafana, Loki, and Tempo. Gave the team visibility into metrics, logs, and traces in one place.

**Outcome:** Developers could diagnose issues quickly. Performance problems were caught before impacting users. Ongoing development became more efficient.

---

## Summary

Enabling delivery means creating the right conditions for the team to succeed: clear backlogs, tooling that removes friction, and quality improvements that build confidence. My experience as a Product Owner and Platform Lead taught me how to translate business needs into actionable work and how to invest in capabilities that pay off over time.

---

[← Back to README](README.md) | [Previous: Architecture](03-architecture.md) | [Next: Stakeholder Relationships →](05-stakeholder-relationships.md)
