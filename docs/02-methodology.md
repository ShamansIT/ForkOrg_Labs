## Methodology
### Research design and approach
This laboratory work will be conducted as a structured assessment and process design within a fictional scenario developed by ForkOrg Labs. 
The methodological framework follows the **IEEE Standard for DevOps: Building Reliable and Secure Systems**, with a focus on the Decision Management process (6.3.3), limited to three subsections: 6.3.3.1 Purpose, 6.3.3.2 Outcomes, and 6.3.3.3 Activities and tasks.
The methodology will combine two complementary components:
A - Gap analysis between the requirements of the standard and current practices, which will be documented in the form of a compliance table;
B - practical demonstration of feasibility in the form of a minimum proof-of-concept (PoC), which will illustrate how decision evidence can be collected and formed into a standardised decision report.
The priority approach in this laboratory decision-making in SDLC, the transparency of evidence, the availability of reproducible rules, and the possibility of further improvement through feedback loops.

### Execution stages according to Decision Management (6.3.3.3)
#### Substage A. Prepare for decisions (6.3.3.3(a))
At the first stage, a decision inventory will be generated - a description of decisions that arise in the life cycle of changes (merge approval, release creation, validate-only execution, deployment attempt, dependency upgrade). For each type of solution, triggers, expected outcomes, and minimum necessary artefacts for justification will be captured.
Next, stakeholder mapping and a simplified RACI matrix for distinguishing roles (responsibility and authority) in decision-making will be performed. Special attention will be paid to the principle of 'decision-making at the lowest feasible level', i.e. determining those decisions that can be delegated to the team or automated without loss of controllability.
To ensure traceability, the Decision Record template will be introduced, which standardizes documentation: decision objective, options, criteria, rationale, assumptions, dependencies, and references to evidence. At the same time, a risk classification model will be formed to define solutions as low, medium or high, which will make it possible to separate solutions suitable for pre-authorisation from solutions that require explicit approval or analysis of alternatives.
At the end of Substage A, a minimum set of security and privacy principles for decision information will be defined, in particular, the avoidance of secrets in logs, the principle of least privilege in relation to access to environments, and control over the distribution of artefacts.

#### Substage B. Gather and analyse decision information, 6.3.3.3(b)
The second stage will be aimed at formalising the decision evidence set - data sufficient to make typical decisions in the process of delivering changes. For validation and deployment decisions, the following signal categories will be defined:
- validation outcomes (e.g., compile/test/metadata checks, where applicable);
- quality signals, including tests and static checks;
- third-party dependency risk signals, where available, including licensing aspects;
- compliance indicators at the level of defined policies.

To unify the review, the decision report format will be established to record the pass/fail conclusion, a brief description of the reasons, and a list of references to artefacts that confirm the conclusion.
To demonstrate practical feasibility, a minimum PoC will be prepared: a containerised preflight run that performs a basic set of checks and generates a decision report as an artefact. The PoC will serve as an example of how automation can support the standard's requirements for data collection and availability 'online and in real time', even if the set of checks at this stage is deliberately limited.

#### Substage C. Make and manage decisions, 6.3.3.3(c)
At the third stage, 'decision strategies' will be defined for different classes of solutions:
automated gate - low-risk changes provided that there is sufficient evidence;
peer review - medium-risk, when automated signals are not enough or expert assessment is required;
formal approval - high-risk, where analysis of alternatives, contingent plans and explicit responsibility is required.
For each strategy, measurable decision criteria will be recorded: thresholds or rules by which 'proceed / defer' conclusions are formed, conditions that require the transition from automation to manual review.
Within this phase, a limited set of alternatives for key solutions will be identified and a way to evaluate them through agreed criteria will be described. The selected decisions are planned to be recorded in the Decision Record, indicating arguments and trade-offs.
Finally, it will offer a feedback loops mechanism to support continuous improvement: collecting data on the results of decisions (failed validations, rollback events, false positives), periodically reviewing them, and correcting rules, thresholds, and hints for teams.

#### Artefacts as an evidence base
As part of the methodology, a set of artifacts will be generated in the repository reflecting the requirements of 6.3.3:
•	decision inventory - a table of decisions, triggers, roles and evidence;
•	RACI / stakeholder map - responsibility and decision-making rights;
•	Decision Record template and example of a completed record;
•	risk classification model as low, medium or high;
•	decision gates policy - minimum rules for pre-authorised decisions;
•	PoC preflight container (docker build/run) with an example of a generated decision report;
•	evidence index, linking requirements, gap analysis results, and specific screenshots or artefacts.
The above artefacts will be used as the basis for the Results section, specifically for the gap analysis table, where the standards will be related to the current state, the identified gap, and the proposed DevOps-oriented action.

