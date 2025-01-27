# Observation-Based-Reasoning-
Observation based reasoning is a novel prompting technique that aims to enhance reasoning capabilities in large and small language models.

Observation-Based Reasoning, a novel prompting technique that enhances LLMs&#39; reasoning
capabilities through structured observation and hypothesis testing. IOR implements a six-step
reasoning process inspired by the scientific method: observation, question generation,
hypothesis formation, testing, refinement, and conclusion. Our approach differs from existing
methods by emphasizing systematic observation before reasoning and incorporating iterative
refinement loops.

IOR Framework Design
The IOR technique implements a structured six-step process:
1. Observation Phase
- Systematic analysis of problem components
- Identification of key relationships and constraints
2. Question Generation
- Formulation of specific queries based on observations
- Development of targeted sub-questions
3. Hypothesis Formation
- Generation of potential explanations
- Construction of logical frameworks
4. Testing Phase
- Systematic verification of hypotheses
- Application of logical rules
5. Refinement Process
- Integration of test results
- Modification of initial hypotheses
6. Conclusion Formation
- Synthesis of refined understanding
- Verification against initial constraints
  
Simple Test Prompt Template

Given a problem, follow these steps:
1. Observation: What do you notice about this problem?
2. Questions: What key questions arise from these observations?
3. Hypothesis: What could explain these observations?
4. Test: Let&#39;s verify this explanation step by step
5. Refine: Based on the test, update your understanding
6. Conclude: Answer the original problem with your refined knowledge
Problem: [Insert test case]
