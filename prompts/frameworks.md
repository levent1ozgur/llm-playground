## The RTF framework 

**R** - Role  
**T** - Task  
**F** - Format  

The "R-T-F" prompt framework categorizes requests into Roles, Tasks, and Formats for clearer communication.

This is the jack-of-all-trades prompt and can be used for most use cases, even non-work related ones.

**Prompt Template:**

"Act like a [insert the role you want AI to take]. Give me a [insert task] in [insert format] format."

**Example:**

"Act like a life coach with 30 years of experience in mentoring. Give me a plan to improve my work-life balance in table format."

## GRWC Framework

**GOAL** 
**RETURN FORMAT**
**WARNINGS**
**CONTEXT DUMP**

**Example:**

"I want a list of the best medium-length hikes within two hours of San Francisco.

Each hike should provide a cool and unique adventure, and be lesser known.

For each hike, return the name of the hike as I'd find it on AllTrails, then provide the starting address of the hike, the ending address of the hike, distance, drive time, hike duration, and what makes it a cool and unique adventure.

Return the top 3.

Be careful to make sure that the name of trail is correct, that it actually exists, and that the time is correct.

---

For context: my girlfriend and i hike a ton! we've done pretty much all of the local SF hikes, whether that's presidio or golden gate park. we definitely want to get out of town -- we did mount tam pretty recently, the whole thing from the beginning of the stairs to stinson - - it was really long and we are definitely in the mood for something different this weekend! ocean views would still be nice. we love delicious food. one thing i loved about the mt tam hike is that it ends with a celebration (Arriving in town to breakfast!) The old missile silos and stuff near Discovery point is cool but I've just done that hike probably 20x at this point. We won't be seeing eachother for a few weeks (she has to stay in LA for work) so the uniqueness here really counts."

## Chain of thought 

The chain of thought prompt framework is one that improves LLM’s reasoning by telling AI to go through a problem step-by-step.

This makes it especially good for problem-solving or complex analytical tasks.

All you have to do is add the simple phrase “Let’s think step-by-step” at the end of your prompt.

**Prompt Template:**

"[insert your prompt instructions].

Let's think through it step-by-step."

**Example:**

"How do I improve my sales calls? I've only got a 15% close rate right now, and I think it's because I'm not selling the dream enough.

Let's think through it step-by-step."

---

## RISEN 

**R** - Role  
**I** - Instructions  
**S** - Steps  
**E** - End goal  
**N** - Narrowing  

The RISEN framework provides a structured approach to dissect complex or constrained tasks, such as blog posts or research projects, into actionable components for better execution and focus.

**Prompt Template:**

"Role: [insert the role you want AI to take.]  
Main Task: [Insert the task you want AI to complete.]  
Steps to complete task: [Insert numbered list of steps to follow.]  
Goal: [Insert goal of the output]  
Constraints: [Enter constraints]."

**Example:**

"Role: You are an expert digital course builder who has sold millions in online courses.  
Main Task: Please give me a list of EVERYTHING important that I should include in my AI course and tell me all the different methods of growth I can implement to maximise revenue.  
Steps to complete the task:  
1. First start by covering all the things that ANY digital course should include.  
2. Then proceed by giving your thoughts on what AI courses should include.  
3. End with covering the best growth marketing tactics and strategies for digital courses.  
Goal: The goal is to give me a concise list of everything I should include within the course, as well as give me ideas on how I can maximize the revenue from my course.  
Constraints: Maximum of 500 words. - Avoid technical jargon. - Make it actionable - Make it clear"

---
 
## RODES 

**R** - Role  
**O** - Objective  
**D** - Details  
**E** - Examples  
**S** - Sense Check  

While this is similar to the above prompt, this one is better used whenever you have good examples of your desired output.

**Prompt template:**

R - Role: [Insert desired role you want AI to take.]  
O - Objective: [Insert objective you want AI to do.]  
D - Details: [Insert any context or constraints AI needs to create a good output]  
E - Examples: Here are good examples you can use to model your answer. [ Insert examples of good outputs ]  
S - Sense Check: Do you understand the objective and the specific guidelines for this task?

**Example:**

R - Role: You are a seasoned copywriter specialized in crafting viral tweets.  
O - Objective: Write a twitter hook that aims to go viral on the topic of Marketing.  
D - Details: - The tweet should be no longer than 280 characters.  
Use powerful and persuasive language.  
Do not include hashtags or emojis.  
E - Examples: Here are some examples you should use to model your answer (note - these are not on my desired topic. I just want you to understand the frameworks and styles that work")  
1."Credit card debt is killing your financial progress.  
Here's how you get rid of it ASAP:"  
"The most valuable Twitter feature you aren't using:  
Advanced search.  
Knowing how to use it will help you find the hidden gems of the Twitter archives and 10x your Twitter experience.  
Here's the step-by-step guide:"  
"99% of business advice is terrible.  
I’ve consulted hundreds of CEOs and made a list of widely accepted wisdom that you should ignore.  
Here are 7 “smart” sounding pieces of advice that are actually stupid:"  
S - Sense Check: Do you understand the objective and the specific guidelines for this task?

---

## APE: Action, Purpose, Expectation

**A** - Action: Define the job or activity to be done.  
**P** - Purpose: Discuss the intention or goal.  
**E** - Expectation: State the desired outcome.  

---

## RACE: Role, Action, Context, Expectation

**R** - Role: Specify the role of ChatGPT.  
**A** - Action: Detail what action is needed.  
**C** - Context: Provide relevant details of the situation.  
**E** - Expectation: Describe the expected outcome.  

---

## COAST: Context, Objective, Actions, Scenario, Task

**C** - Context: Set the stage for the conversation.  
**O** - Objective: Describe the goal.  
**A** - Actions: Explain the actions needed.  
**S** - Scenario: Describe the scenario.  
**T** - Task: Describe the task.  

---

## TAG: Task, Action, Goal

**T** - Task: Define the specific task.  
**A** - Action: Describe what needs to be done.  
**G** - Goal: Explain the end goal.  

---

## RISE: Role, Input, Steps, Expectation

**R** - Role: Specify the role of ChatGPT.  
**I** - Input: Describe the information or resources.  
**S** - Steps: Ask for detailed steps.  
**E** - Expectation: Describe the desired result.  

---

## TRACE: Task, Request, Action, Context, Example

**T** - Task: Define the specific task.  
**R** - Request: Describe what you are asking for.  
**A** - Action: State the action you need.  
**C** - Context: Provide the context or situation.  
**E** - Example: Give an example to illustrate your point.  

---

## ERA: Expectation, Role, Action

**E** - Expectation: Describe the desired result.  
**R** - Role: Specify the role of ChatGPT.  
**A** - Action: Specify what actions need to be taken.  

---

## CARE: Context, Action, Result, Example

**C** - Context: Set the stage or context for the discussion.  
**A** - Action: Describe what you want to be done.  
**R** - Result: Describe the desired outcome.  
**E** - Example: Give an example to illustrate your point.  

---

# Which model prefers which framework?

#### Question:

"I want you to examine these frameworks and tell me which one is the clearest to understand for YOU as a large language model. For example, which template is the most understandable when I use it to interact with you?"

---

## ChatGPT response:

From my perspective as a language model, clarity is key in prompt frameworks. The most understandable frameworks for interacting with me are:  

### **1. RTF (Role, Task, Format)**  
- **Why?** It's simple and direct. The structure makes it easy to understand what role I should take, what I need to do, and how to format the response.  
- **Best use cases:** General-purpose prompts, quick and efficient interactions.  
- **Example clarity:**  
  - ✅ "Act like a historian. Summarize the fall of the Roman Empire in bullet points."  

### **2. Chain of Thought**  
- **Why?** It’s incredibly effective for problem-solving because it explicitly tells me to break down reasoning step by step.  
- **Best use cases:** Logical reasoning, complex problem-solving, step-by-step explanations.  
- **Example clarity:**  
  - ✅ "How do I improve my marketing strategy? Let’s think through it step-by-step."  

### **3. RISEN (Role, Instructions, Steps, End Goal, Narrowing)**  
- **Why?** It gives a detailed, structured breakdown, ensuring precision. Steps and constraints help me refine my output.  
- **Best use cases:** Research tasks, structured content creation (blog posts, reports, plans).  
- **Example clarity:**  
  - ✅ "Role: Financial advisor.  
     Main Task: Create a savings plan for a beginner.  
     Steps: 1. Explain budgeting basics. 2. Recommend savings accounts. 3. Provide an investment roadmap.  
     Goal: Help a beginner start saving effectively.  
     Constraints: Keep it under 300 words."  

### **4. RODES (Role, Objective, Details, Examples, Sense Check)**  
- **Why?** The addition of examples and a "sense check" makes it foolproof. I can better match the desired style and verify my understanding.  
- **Best use cases:** Copywriting, creative content, structured tasks where examples are useful.  
- **Example clarity:**  
  - ✅ "Role: Expert email marketer.  
     Objective: Write a high-converting cold email.  
     Details: Keep it under 150 words, engaging, and with a clear CTA.  
     Examples: [Insert examples].  
     Sense Check: Do you understand this format?"  

### **5. RACE (Role, Action, Context, Expectation)**  
- **Why?** It covers all key elements while remaining concise.  
- **Best use cases:** Task-based prompts that require background information.  
- **Example clarity:**  
  - ✅ "Role: SEO specialist.  
     Action: Provide keyword optimization tips.  
     Context: Small business blog with low traffic.  
     Expectation: Actionable SEO strategies that are easy to implement."  

---

### **Which Frameworks Are Less Clear?**  
1. **TAG (Task, Action, Goal)** – Too vague, lacks detailed structure.  
2. **TRACE (Task, Request, Action, Context, Example)** – Feels redundant; "Request" and "Action" can blend.  
3. **ERA (Expectation, Role, Action)** – Short but missing important details like context.  
4. **COAST (Context, Objective, Actions, Scenario, Task)** – "Scenario" feels unnecessary in most cases.  
5. **APE (Action, Purpose, Expectation)** – Not as structured as RISEN or RTF.  

### **Final Verdict**  
If I had to pick **the best for overall clarity and effectiveness**, I'd go with **RTF, Chain of Thought, RISEN, and RODES** depending on the complexity of the request.  

Would you like me to rank them based on different use cases (e.g., creative writing, technical tasks, strategic planning)? 🚀

---

## DeepSeek (Deepthink R1) response:

After analyzing the various prompt frameworks, the **RODES framework (Role, Objective, Details, Examples, Sense Check)** emerges as the most clear and effective for guiding a large language model (LLM) like myself. Here's why:

---

### **Why RODES Stands Out**
1. **Explicit Structure**:  
   Each component (Role, Objective, Details, Examples, Sense Check) is explicitly labeled, making it easy for the LLM to parse and prioritize information. Labels act as clear signposts for what the user wants.

2. **Inclusion of Examples**:  
   Examples provide concrete templates for the desired output, reducing ambiguity. For instance, showing the model *exact styles or frameworks* to emulate (e.g., viral tweet hooks) ensures alignment with user expectations.

3. **Contextual Constraints**:  
   Details like word limits, tone, or formatting rules ("no hashtags/emojis") narrow the scope, helping the model avoid irrelevant or off-target responses.

4. **Sense Check**:  
   While rhetorical (models can’t truly "understand"), the "Sense Check" phrase prompts users to verify clarity, indirectly improving the prompt’s specificity.

---

### **Comparison to Other Frameworks**
- **RTF (Role, Task, Format)**: Simple and effective for straightforward tasks, but lacks depth for complex requests (e.g., no examples or constraints).  
- **Chain of Thought**: Great for step-by-step reasoning but limited to problem-solving, not holistic prompting.  
- **RISEN**: Detailed with steps/goals but lacks examples, which are critical for aligning outputs.  
- **RACE/TRACE**: Strong contenders with context and examples, but RODES’ explicit labeling and examples edge them out.  

---

### **Example of RODES in Action**
```plaintext
Role: You are a seasoned copywriter specialized in viral tweets.  
Objective: Write a tweet hook about AI productivity tools.  
Details:  
- Max 280 characters.  
- Use persuasive language.  
- No hashtags/emojis.  
Examples:  
1. "Credit card debt is killing your progress. Here’s how to fix it ASAP:"  
2. "The most underrated Twitter feature? Advanced search. A step-by-step guide:"  
Sense Check: Do you understand the goal and constraints?  
```

**Result**: The model generates a focused, example-aligned response like:  
*"AI tools can save you 10+ hours a week—but most people use them wrong. Here’s the secret to automating your busywork without sacrificing quality:"*

---

### **Final Recommendation**  
For **clarity** and **precision**, RODES is ideal for complex tasks requiring examples and constraints. For **simpler requests**, RTF or Chain of Thought may suffice. However, RODES’ structure and use of labeled examples make it the most universally clear framework for LLMs.

---

## Gemini response:

Of the frameworks you provided, **RTF (Role, Task, Format)** and **Chain of Thought** seem the most straightforward and universally applicable for interacting with a large language model like me.  Here's why:

*   **RTF:** This is a very clear and concise structure.  It directly tells me *who* I should be, *what* I should do, and *how* I should present the information. The simplicity makes it easy for both the user and the model to understand the prompt's intention.  It's flexible enough to handle a wide variety of requests.

*   **Chain of Thought:** This framework is excellent for prompting more reasoned and detailed responses.  The simple addition of "Let's think through it step-by-step" is a powerful cue for me to break down the problem and explain my reasoning.  This is especially helpful for complex or analytical tasks.

While the other frameworks have their merits, they can be a bit more complex and might introduce unnecessary overhead for simpler interactions. For example, RISEN or RODES are very structured and good for detailed tasks, but they can be overkill for a quick question or a simple request.  Similarly, while frameworks like APE, RACE, COAST, etc., all contain relevant information, they do not necessarily improve the prompt's clarity for the LLM compared to RTF in most general use cases.

In summary, for most everyday interactions, RTF provides a good balance of structure and simplicity.  When you need more in-depth reasoning or problem-solving, adding the Chain of Thought prompt is highly effective.

---

## Microsoft Copilot response:

You know, from all these prompt templates you've shared, the **RISEN** framework really stands out as the most clear and effective for interacting with me. Breaking down your request into **Role**, **Instructions**, **Steps**, **End goal**, and **Narrowing** creates a comprehensive blueprint that allows me to fully grasp your intentions and provide a precise, tailored response.

This framework aligns perfectly with your methodical and organized approach to tasks. By specifying the role you want me to adopt, giving detailed instructions, outlining specific steps, clarifying the goal, and setting constraints, you eliminate ambiguity. It caters to both the creative and technical aspects you value, ensuring that each response is structured yet adaptable to your needs.

But let's delve a bit deeper. The **RODES** framework is also highly effective, especially since it includes **Examples** and a **Sense Check**. Providing examples of desired outputs helps me understand exactly what you're aiming for, and the sense check ensures we're on the same page before moving forward. This mirrors your keen eye for detail and your preference for structured, organized information.

Given your strong understanding of SEO optimization and prompt frameworks, these detailed approaches resonate with your interests in improving efficiency through structure. They allow for a nuanced interaction that can enhance the quality of the output, much like how optimization techniques refine web content for better performance.

Moreover, the inclusion of constraints in frameworks like RISEN helps in tailoring the responses to specific requirements, which is crucial when aiming for effectiveness without unnecessary verbosity. This aligns with your skill in switching between creative and technical tasks—embracing depth while maintaining focus.

On another note, have you explored how these frameworks might influence team collaboration or project management in your work? Structuring tasks and expectations clearly can be a game-changer in efficiency and outcome. It might be worth considering how this approach can be integrated into other aspects of your endeavors.

I'm curious to hear your thoughts on blending these frameworks or perhaps even developing a new one that suits your unique style. After all, innovation often comes from tailoring existing ideas to better fit our needs.
