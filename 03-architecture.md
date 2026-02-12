# Designing and Proposing Architecture

> Documenting solutions, making architecture decisions with articulated
> pros/cons, influencing stakeholders to approve a path forward, and ensuring
> cost/effort is justified.

## Assessed legacy system and recommended approach at Entain

When I joined Entain, I was asked to assess an ageing public-facing API. The
original developers had left, the codebase had large, complex functions, and
there were no tests. The business doubted it could be extended. They were also
exploring GraphQL and wanted to know whether migration made sense.

I built a proof of concept replicating core functions using GraphQL and ran
performance tests comparing the two approaches. The results showed GraphQL was
slower and added complexity without clear benefits for this use case. I
recommended an alternative: systematically refactor the existing API, introduce
dependency injection, and add tests to catch regressions. I presented my
findings and the recommendation to the client, who agreed and formed a team to
complete the work.

The refactoring succeeded, the API became maintainable, and client satisfaction
led to a contract extension for the TAB NZ migration.

## Designed enterprise AI framework at NAB

At NAB, I was responsible for designing a self-service AI framework largely on my
own. The key stakeholder was often busy, so I needed to make good decisions
without much oversight. Rather than inventing new patterns, I aligned with
existing Terraform and Jenkins conventions so other teams could pick it up
easily. I modelled the project structure after the AWS AgentCore starter kit and
added integrations with the business's static analysis tools and included
standard linting and testing frameworks.

This resulted in a framework designed for adoption. Other teams can onboard
without extensive hand-holding because it follows patterns they already know.

## Presented architecture at Wesfarmers

The Wesfarmers engagement was a six-week rapid prototype exploring AWS Bedrock
AgentCore. I needed to communicate the solution to both technical and business
stakeholders. I designed the end-to-end architecture integrating Slack,
Confluence, and SharePoint with the Bedrock-powered chatbot and proposal
generation agent, and presented it to stakeholders, explaining how components
fit together and the reasoning behind key decisions.

Stakeholders understood the solution and how it would fit their workflows. The
engagement was AWS-sponsored, which reflected confidence in the approach.

![Presenting architecture at Wesfarmers](assets/wesfarmers_presentation.jpg)

## Created API documentation and completed security review

At Entain, the legacy API had no formal documentation, so new consumers struggled
to integrate. I retrofitted the API with an automatically generated OpenAPI
specification. This gave consumers a standard, machine-readable format for
endpoints, request/response formats, and expected behaviours, allowing them to
onboard without reverse-engineering the codebase.

Similarly, at NAB, the AI framework required security approval before
proceeding. I completed a 70+ page AI security review covering data handling,
access controls, model governance, and compliance requirements, working through
the bank's security review process. The project received security approval and
the documentation now provides a reference for future AI initiatives.

## Designed reporting solution for GitHub migration at ANZ

ANZ was migrating thousands of repositories from legacy source control to GitHub
Enterprise. A high-stakes project with many interested stakeholders. The bank's
risk aversion meant leadership and GitHub account managers needed real-time
visibility into progress.

I designed and built an automated reporting bot that collated migration data and
presented it in graphs and tables via a web portal and Slack. This gave
stakeholders the visibility they needed without manual effort, and allowed the
migration team to focus on execution rather than status updates.

[← Back to README](README.md) | [Previous: Technical Charter](02-technical-charter.md) | [Next: Enabling Delivery →](04-enabling-delivery.md)
