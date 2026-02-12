# Enabling Team Delivery

> Ensuring issues/risks are identified with sufficient time, building backlogs
> with clear acceptance criteria, protecting team focus time, and investing in
> efficiency improvements.

## Led platform strategy and backlog creation (Platform Lead)

At Fred, development environments were created manually, making them inconsistent
and long-lived because people were afraid to delete anything. This led to low
confidence, as environments were a poor representation of production, which in
turn slowed delivery due to risk aversion around releases. We also had poor
visibility of cloud costs, with no clear ownership or justification for running
instances.

I worked with the business to create a platform uplift strategy. We implemented
infrastructure-as-code with Terraform and clear tagging, which allowed us to
treat environments as disposable, consistent assets. This increased confidence,
reduced costs, and increased delivery velocity. I created and prioritised the
backlog, got stakeholder buy-in, and broke features into actionable work. The
team moved from manual deployments to a repeatable, scalable platform.

## Refined backlog into deliverable work at Entain

After the Entain API team formed, we had a Product Owner prioritising features,
but business priorities still needed translating into work developers could pick
up.

I worked with the team to refine the backlog into deliverable user stories and
broke down feature areas including observability uplift, performance
improvements, OpenAPI documentation, and new API endpoints. Developers had
clarity on what to build and why, work was sized appropriately with clear
acceptance criteria, and the team could focus on delivery rather than constantly
seeking clarification.

## Built self-service tooling at NAB

At NAB, AI initiatives were blocked waiting for the platform team to provision
infrastructure and configure deployments, which slowed adoption across the
organisation and created a bottleneck for the platform team.

I designed a self-service framework so teams could build and deploy Bedrock
AgentCore applications independently. I created opinionated templates with
schema-validated configuration and automated pipelines that handled the full
deployment lifecycle, aligned with existing Terraform and Jenkins patterns so
teams didn't need to learn new conventions. Teams can now deploy without waiting
on the platform team, and the workload and bottleneck on the platform team have
been alleviated. The investment in tooling reduces friction for every new AI
initiative going forward.

## Drove quality improvements at Entain

The legacy Entain API had no tests, so any change risked regressions and slowed
delivery. Automated testing wasn't part of the company's culture. I didn't walk
past it. I worked with our team to convince them that the initial effort would
pay off with faster, more confident delivery in the long run.

I championed a quality-first approach during the refactoring, introduced
dependency injection to make the codebase testable, and established testing
patterns. Unit test coverage increased from 0% to 75%. The team could make
changes with confidence, and our project served as a positive example for
driving cultural change with their leadership.

## Set up observability at Entain

Without visibility into system behaviour, debugging was time-consuming and
developers couldn't see performance characteristics or trace issues easily.

I set up observability dashboards using Prometheus, Grafana, Loki, and Tempo,
giving the team visibility into metrics, logs, and traces in one place.
Developers could diagnose issues quickly, performance problems were caught
before impacting users, and ongoing development became more efficient.

## Identified risks early at ANZ

At ANZ, I was tasked with assessing the scope of migrating CI pipelines from
Bamboo to GitHub Actions. Analysis of the Bamboo database revealed hundreds of
VMs running Bamboo deployment agents across the bank, with limited understanding of ownership or purpose.

I built scripts integrating with internal systems to surface this information
and consolidated it into reports. This gave the bank visibility they'd never
had, enabled ~30% of the VMs to be deprovisioned, and reduced the risk profile
for the migration. Identifying this early meant we could proceed with a clearer
picture of what we were dealing with.

[← Back to README](README.md) | [Previous: Architecture](02-architecture.md) | [Next: Stakeholder Relationships →](04-stakeholder-relationships.md)
