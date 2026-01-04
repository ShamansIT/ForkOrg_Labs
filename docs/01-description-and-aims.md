## Description and Aims

**ForkOrg Labs** is a fictional organisation within this lab, which plans to implement an internal **developer workflow** aimed at reducing the internal feedback loop during development in Salesforce: edit -> validate -> fix.
The proposed approach involves the introduction of a containerised **'preflight' stage**, which forms the evidence base necessary for decision-making before performing any deployment or merge actions.

According to the conditional scenario, the organisation **ForkOrg Labs** already partially applies **DevOps** practices - version control, peer review, basic CI checks. However, the quality of the decision-making process differs significantly between teams: risks are interpreted ambiguously, approval thresholds are not clearly defined, and the rationale for decisions on releases is not recorded in a form suitable for reuse. As a result, this leads to unnecessary rework, unsuccessful validations, and poor traceability of the reasons why certain changes were advanced further along the life cycle.

This lab uses the IEEE Standard for DevOps, with a focus on the Decision Management process (Section 6.3.3). The work begins with a gap analysis between the requirements of the standard and current practice, followed by a practical approach to improving the quality of SDLC by unifying evidence, clearly delineating decision-making powers, and automating where appropriate.

### Objectives of laboratory work:
1.	Conduct a gap analysis between the requirements of **IEEE DevOps Decision Management (6.3.3)** and current decision-making practices in ForkOrg Labs.
2.	Develop a workable approach to decision management that supports faster, evidence-based decisions and improves traceability throughout the lifecycle.
3.	Identify the types of solutions that can be **pre-authorised** and implemented in the form of automated gates for low-risk changes.
4.	Describe the **minimum set of evidence** required to support decision-making and form effective feedback loops for continuous improvement.

### Note: IEEE as engeniring standart

**IEEE 2675-2021 (Standard for DevOps: Building Reliable and Secure Systems)** is a fundamental international standard that formalises DevOps as a holistic engineering discipline. The need for its development arose due to a critical discrepancy between the rapid development of Agile practices and the need to ensure high reliability in regulated industries. Until its introduction in 2021, **the term 'DevOps'** was often interpreted subjectively, making it difficult to certify and audit processes in large organisations. The standard is the result of many years of cooperation between **IEEE** and **ISO** experts in order to adapt the classic standards of the software development life cycle to the conditions of continuous integration and deployment.

The scientific and practical value of this standard lies in the clear definition of requirements for the processes of synthesis and verification of systems, where special emphasis is placed on the 'left-shift' approach. By implementing **DevSecOps** early quality control and security mechanisms, the standard provides conceptual integrity between iterative development and classical systems engineering. This allows organisations to transform informal arrangements into verified processes that provide full traceability for the management of the development process

The use of IEEE 2675-2021 (IEEE Standard for DevOps) in this lab work is due to its transition from purely cultural aspects of DevOps to rigorous engineering requirements.
