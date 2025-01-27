# Observation-Based-Reasoning                                                                                     Author: Rish Midha 

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
4. Test: Lets verify this explanation step by step
5. Refine: Based on the test, update your understanding
6. Conclude: Answer the original problem with your refined knowledge
Problem: [Insert test case]

Our initial test results show promosing results. We tested our prompting technoique on the notorious alice in wonderland problem where "alice has x brothers and y sisters. how many sisters does alice's brother have? We used claude 3.5 sonnet at base prompt and received an incorrect answer. We then used claude 3.5 haiku with our observation based reasoning technique and received the correct answer. We then asked multiple logical, reasoing  & cause and effect relationship questions & saw a siginficant increase in the answer quality.

Our results show that by mimicing the scientific discovery method. The model is able to create hypothesis based on the observations. The hypothesis might hallucinate but by verifying it with facts & logic in the refine section. We force the model to correct itself before presenting the final conclusion making the model more reliable and hallucinate less. 

Future work:
1) Validating on benchmark datasets like multi-logi eval, big bench hard, etc.
2) Comparing it to COT & TOT.
3) Fine tuning the model to teach it different types ofquestions to ask in different cases.
4) Use the same principals with a multimodal or physics informed neural network, place it in a stimulation and feed it observations and ask the model questions to check it's understanding of the observations.
5) Give the models extarnal tools to aid in the testing part.(React 2023)

   References
   Chain of thought paper, Tree of thought paper, React Paper (2023)
