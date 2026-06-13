# GenAI Production Readiness Checklist

A practical checklist for reviewing whether a GenAI system is ready to move beyond demo or prototype stage.

This is a working checklist, not a final production framework. I use it to structure the questions I would ask before recommending or approving a GenAI system for production use.

The checklist is intentionally broad. Some items apply more to RAG systems, some to agentic systems, and some to simple LLM-powered applications. The goal is to avoid treating the model alone as the whole solution.

## 1. Business and use-case clarity

* [ ] The business problem is clearly defined.
* [ ] The target users are identified.
* [ ] The expected outcome is measurable.
* [ ] The system has a clear owner.
* [ ] The use case is valuable enough to justify cost, risk, and maintenance.

## 2. Data readiness

* [ ] Required data sources are identified.
* [ ] Data access permissions are understood.
* [ ] Sensitive data handling is documented.
* [ ] Data quality issues are known.
* [ ] Data refresh requirements are defined.
* [ ] Retention and deletion requirements are understood.

## 3. Model and architecture choice

* [ ] The model choice is justified.
* [ ] Cloud vs local model deployment has been evaluated.
* [ ] Latency expectations are realistic.
* [ ] Cost expectations are estimated.
* [ ] Context window limits are understood.
* [ ] Fallback behavior is defined.
* [ ] Vendor/API dependency risks are reviewed.
* [ ] Provider rate limits, quotas, and SLA expectations are understood.
* [ ] Model deprecation or forced upgrade risks are considered.
* [ ] Provider outage fallback options are defined.

## 4. Security, governance, and guardrails

* [ ] Authentication and authorization are defined.
* [ ] Access to prompts, outputs, logs, and documents is controlled.
* [ ] Sensitive information is not unnecessarily exposed to the model.
* [ ] Prompt injection risks have been reviewed.
* [ ] Input filtering requirements are defined.
* [ ] Output filtering requirements are defined.
* [ ] PII leakage risks in model outputs are reviewed.
* [ ] Content safety guardrails are defined where needed.
* [ ] Off-topic, unsafe, or unauthorized request handling is defined.
* [ ] Audit and logging requirements are defined.
* [ ] Compliance requirements are reviewed.

## 5. Evaluation and quality

* [ ] A test set exists for expected user queries.
* [ ] Failure cases are documented.
* [ ] Hallucination risk is evaluated.
* [ ] Output quality is measured.
* [ ] Regression testing is planned.
* [ ] Human review is defined for high-risk outputs.
* [ ] Evaluation criteria are documented.
* [ ] Evaluation results are tracked over time.

## 6. Operations and LLMOps

* [ ] Monitoring is planned.
* [ ] Cost tracking is planned.
* [ ] Latency tracking is planned.
* [ ] Error handling is defined.
* [ ] Rollback procedures exist.
* [ ] Model/version changes are tracked.
* [ ] Prompt versions are tracked.
* [ ] Prompt changes are tested before release.
* [ ] Prompt changes follow a change-management process.
* [ ] Provider/API changes are monitored.
* [ ] Incident response procedures exist for harmful, incorrect, or high-impact outputs.
* [ ] Ownership between business, engineering, security, and operations is clear.

## 7. User experience

* [ ] The user knows when they are interacting with AI.
* [ ] The system explains uncertainty where needed.
* [ ] The system avoids overconfident answers.
* [ ] Users have a way to report bad outputs.
* [ ] Escalation to a human process exists where needed.

## 8. Launch decision

* [ ] Known risks are documented.
* [ ] Go/no-go criteria are defined.
* [ ] Stakeholders have approved the launch.
* [ ] Post-launch review is scheduled.
