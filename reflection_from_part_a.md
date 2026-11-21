# Reflection from Part A

_Concept Analysis (not more than 500 words)_

## i. What is Agentic Software Engineering?
Start with the two words separately. Software engineering is the disciplined way of building software, covering specification, development, validation, and evolution so that a system works and keeps working (Sommerville, 2016, Ch. 1-2). An agent, in Russell and Norvig's terms (Ch. 2), is something that perceives its environment and acts on it to reach a goal. Put together, Agentic Software Engineering means building software with agents that take part in the work itself. Given a goal, an agent can break it into steps, write and test code, use tools like a repository or terminal, and revise based on the results, while people set the goals, review the output, and make the final calls.

## ii. How does an AI agent differ from a traditional software application?
A traditional program follows rules someone wrote in advance. A test script, for example, runs the same checks the same way every time. An AI agent gets a broader objective, such as "keep the build green." It can read a failing test, investigate the code, propose a fix, rerun the tests, and try again if that fails. So the real difference is how decisions are made: fixed rules and predictable output versus goal, reasoning, action, and evaluation. That does not make agents better everywhere. Where safety and consistency matter most, such as a medical device controller, plain deterministic software is still the safer choice (Sommerville, 2016).

## iii. Why are Agile methods appropriate for developing agentic systems?
Nobody can fully predict what an agent will do until it is running, so requirements keep shifting. Agile is built for that. Incremental delivery and frequent feedback (Sommerville, 2016, Ch. 2) let a team release something small, watch how the agent behaves, and adjust. In Scrum, the Sprint Review and Retrospective (Scrum Guide, 2020) are natural checkpoints where people inspect what the agent produced and decide what to change. Git supports this by recording every change, including the ones agents make, so anything can be reviewed or rolled back.

## iv. What risks should developers consider when deploying autonomous AI agents?
Developers should think about safety, security, privacy, and ethics. An agent acting alone can make a wrong decision with real consequences, like deleting data or pushing broken code. Security risks include excessive permissions, leaked credentials, and prompt injection, where malicious text in the agent's input tricks it into misusing its tools. Privacy is at risk whenever personal data ends up in prompts or logs. Bias, over-reliance, and unclear accountability matter too. The NIST AI Risk Management Framework (2023) treats these as risks to be governed.

## v. Why is human oversight important in AI-enabled applications?
AI can be wrong while sounding completely sure, so someone has to check. Human oversight keeps accountability with people, catches errors before they spread, and lines up with the Govern function of the NIST AI RMF, which calls for clear roles and responsibilities. In practice, agents propose and humans approve anything high-impact.

## What I learned
Writing this showed me that agentic systems shift engineering from predictable behavior to managed behavior. Because agents decide their own actions, good practice depends on iteration (Agile), traceability (Git), and human accountability (oversight and governance).
