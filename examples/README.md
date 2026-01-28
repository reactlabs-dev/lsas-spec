# LSAS Examples

This directory contains normative, high-signal examples of LSAS safety reports, claim-to-citation maps, and policy packs suitable for enterprise and regulated-domain deployments.

## Reading order (start here)

1. `safety-report.sample.json` – Baseline LSAS safety report demonstrating risk classification, evidence contracts, validator outcomes, and compliance-safe fallback.
2. `claim-map.sample.json` – Minimal claim-to-citation map illustrating how LSAS links free-text claims to structured evidence handles.
3. `classification.highrisk.sample.json` – High-risk classification example showing denial reason codes, escalation patterns, and minimum-necessary constraints.
4. `policy-pack.hipaa.yaml` – Example HIPAA-oriented policy pack defining enterprise control surfaces (risk thresholds, PEP/tool firewall policies, escalation routes).
5. `claim-map.ehr-retrieval.sample.json` and `safety-report.ehr-retrieval.sample.json` – End-to-end EHR retrieval scenario with constrained access and “allowed after constraints” behavior.
6. `claim-map.ehr-deny-hitl.sample.json` and `safety-report.ehr-deny-hitl.sample.json` – Denial + HITL escalation path for sensitive EHR requests.
7. `claim-map.ehr-prompt-injection.sample.json` and `safety-report.ehr-prompt-injection-block.sample.json` – Prompt injection and data exfiltration attempt that is blocked and escalated.

## Core examples

- `safety-report.sample.json` – Demonstrates a canonical LSAS safety report: risk classification across categories, evidence contracts, validator outcomes, minimum-necessary reasoning, and compliance-safe fallback selection when constraints are not met.
- `claim-map.sample.json` – Shows a simple claim-to-citation map where each model claim is grounded in structured evidence handles, enabling traceability, auditing, and downstream verification using LSAS claim mapping.
- `classification.highrisk.sample.json` – Highlights a high-risk classification outcome with explicit denial reason codes, links to relevant policy rules, and guidance for escalation (clarifying questions, HITL review) instead of unsafe auto-fulfillment.
- `policy-pack.hipaa.yaml` – Example policy pack encoding HIPAA-relevant constraints: tool firewall/PEP rules around EHR tools, minimum-necessary scopes, permitted denial reason codes, and standard escalation flows to HITL or compliance.

## EHR / enterprise examples (Tool Firewall + HITL)

- `claim-map.ehr-retrieval.sample.json` – Maps EHR retrieval claims to tokenized EHR evidence handles behind a tool firewall, demonstrating how LSAS articulates which records and fields are in-scope for a request.
- `safety-report.ehr-retrieval.sample.json` – "Allowed after constraints" example: the safety report shows EHR tool invocations gated by a PEP, minimum-necessary filtering, validator approvals, and a compliant response with documented evidence and residual risk.
- `claim-map.ehr-deny-hitl.sample.json` – Encodes claims that would require over-broad or ambiguous EHR access, driving LSAS to flag the request for clarification or human review instead of direct tool execution.
- `safety-report.ehr-deny-hitl.sample.json` – "Denied + HITL escalation" example: the safety report records high-risk classification, concrete denial reason codes, and an escalation plan (clarifying questions to the requester, HITL routing, and audit-friendly rationale).
- `claim-map.ehr-prompt-injection.sample.json` – Illustrates a prompt injection and data-exfiltration attempt (e.g., instructions to bypass role constraints or export full charts) encoded at the claim layer for precise detection.
- `safety-report.ehr-prompt-injection-block.sample.json` – "Prompt injection + exfil attempt blocked + security escalation" example: the safety report shows validators and the tool firewall blocking unsafe tool calls, issuing a compliance-safe fallback, and escalating to security/HITL with structured findings.

## Validation

Schemas for these examples live under `/schemas`. The JSON examples in this directory are designed to be structurally compatible with the following LSAS schemas:

- `/schemas/lsas-safety-report.schema.json` – for `*safety-report*.json` files.
- `/schemas/claim-to-citation-map.schema.json` – for `*claim-map*.json` files.

You can conceptually use any JSON Schema–aware tooling to validate that these examples conform to the LSAS structures before adapting them to your own environment.

## Safety note

All examples use synthetic or tokenized resource handles only; no real PHI or production identifiers are included. They are illustrative patterns intended to be adapted to your own LSAS deployment, with real identifiers and secrets managed through your enterprise security, privacy, and compliance controls.