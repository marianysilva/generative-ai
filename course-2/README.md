# IBM - Generative AI for Data Engineers Specialization

## Course 2 - Generative AI: Prompt Engineering Basics

## Module 1

### Exploring Prompt Engineering in Generative AI

- Optimizing model efficiency: Prompt engineering helps design intelligent prompts that allow the users to harness the full capabilities of these models without requiring extensive retraining

- Boosting performance for specific tasks: Prompt engineering empowers generative AI models to deliver responses that are nuanced and have a context, rendering them more effective for specific tasks.

- Understanding model constraints: Refining prompts through each iteration and studying the corresponding responses of the model can help us understand its strengths and weaknesses. This knowledge can further guide feature enhancement or complete development of the model in the future.

- Enhancing model security: Skilled prompt engineering can prevent issues of harmful content generation due to poorly designed prompts, thereby enhancing safe utilization of the model.

### Well-crafted prompt 

A well-crafted prompt consists of four key building blocks that guide the AI model to generate the desired output:

- **Instructions** serve as the core directive that tells the model exactly what you want it to do. Think of instructions as a clear set of commands that steer the AI's behavior.

        "Write an essay in 600 words, analyzing the impact of artificial intelligence on healthcare."

- **Context** provides the critical background information that frames the instruction. This helps the model understand the broader situation and generate more relevant responses. Consider how adding context enriches our previous example:

        "In the last decade, artificial intelligence has rapidly evolved from experimental technologies to practical applications in clinical settings. These systems are now being deployed for diagnostics, treatment planning, and administrative tasks. Write an essay in 600 words analyzing the impact of artificial intelligence on healthcare."

The added context about climate changes helps the model better understand the scope and focus of the requested analysis.

- **Input data** represents specific information or references you provide to help shape the model's response. This could be facts, figures, or other concrete details that should inform the output. For instance, our prompt becomes more focused with added input data:

        "You have been provided with recent statistics on AI diagnostic accuracy compared to human physicians across five major specialties (radiology, pathology, dermatology, ophthalmology, and cardiology). Write an essay in 600 words, analyzing the impact of artificial intelligence on healthcare diagnostics."

- Finally, **output indicators** specify the characteristics you want to see in the model's response. These could include length, style, tone, or format requirements.

        "In the last decade, artificial intelligence has rapidly evolved from experimental technologies to practical applications in clinical settings. You have been provided with recent statistics on AI diagnostic accuracy compared to human physicians across five major specialties. Write an analytical essay in 600 words on the impact of artificial intelligence on healthcare diagnostics. Include specific examples from at least three specialties, incorporate comparative accuracy statistics, and conclude with ethical considerations and future implications for medical professionals."

When crafting prompts, think of these elements as working together like ingredients in a recipe. The **instructions** tell the model what to make, the **context** sets the stage, the **input data** provides the raw materials, and the **output indicators** describe how the final product should look and feel. Understanding how to combine these elements effectively will help you get more precise and useful responses from AI models.

Best practices for writing effective prompts can be implemented across four dimensions:

- **Clarity** includes using simple and concise language; avoide jargon and complex terms; provide explicit instructions
- **Context** provides background and required details
- **Precision** means being specific and providing examples
- **Role play** can enhance responses by assuming a persona and offering relevant context.

These practices can be adapted to specific needs for optimal results.

### Prompting Tools

Prompt engineering tools provide various features and functionalities to optimize the creation of prompts for desired outcomes. These tools are specifically useful for users who may not be proficient with natural language processing or NLP techniques, but want to achieve specific outcomes when using generative AI models. 

Some of these functionalities include:
- Suggestions for prompts
- Contextual understanding
- Iterative refinement
- Bias mitigation
- Domain-specific aid
- Libraries of predefined prompts

A few common tools and platforms for prompt engineering include:
- IBM Watsonx.ai
- Prompt Lab
- Spellbook
- Dust
- PromptPerfect

**Ask the model for help:** When unsure how to formulate a prompt, ask the model itself what would be the best approach.

## Module 2

### Prompting Techniques

- **Task Specification** - Explicitly stating the objective to increase accuracy (e.g., "Translate this English sentence into French")
- **Contextual Guidance** - Providing specific instructions to generate relevant output (e.g., specifying "highlighting its iconic landmarks" when asking about New York City)
- **Domain Expertise** - Using specialized terminology for fields like medicine, law, or engineering
- **Bias Mitigation** - Giving explicit instructions to generate neutral responses (e.g., "without favoring any gender")
- **Framing** - Guiding LLMs to generate responses within required boundaries (e.g., specifying word count and focus areas)
- **Zero-Shot Prompting** - Asking the model to perform a task without providing examples, relying on its pre-trained knowledge (common in everyday ChatGPT usage)
- **Few-Shot Prompting** - Providing 2-3 examples to guide the model toward the desired output format or approach (examples need only be properly formatted, not necessarily correct)
- **Chain of Thought** - Guiding the model through a sequential series of steps to help it stay on track for complex problem-solving tasks
- **Role Assignment** - Instructing the model to adopt a specific expert persona (e.g., JavaScript developer, CEO, product manager) to improve output quality and relevance
- **User Feedback Loop** - Iteratively refining prompts based on LLM responses until achieving desired results

### Interview Pattern Approach
The interview pattern approach to prompt engineering simulates a conversational interview style with AI models to produce more specific and tailored responses.

- **Meticulous Prompt Optimization** - Designing prompts specifically to meet precise objectives
- **Follow-up Question Structure** - Providing instructions that prompt the model to ask necessary follow-up questions
- **Information Processing** - Model draws relevant information from user responses, processes it, and delivers an optimized response
- **Information Quality** - The more detailed information provided, the better the results

#### Example Application:

    "You will act as a seasoned financial advisor. Your objective is to engage in a comprehensive financial planning session with me. Begin by asking a series of detailed questions, one at a time, to gather all the essential information required to craft the most tailored and effective financial plan based on my specific goals, risk tolerance, and current financial situation."

Model's Response: The model asks targeted questions.

#### Benefits Over Conventional Prompting:

- Creates a more dynamic and iterative conversation
- Replaces static, one-time prompts with information exchange
- Clarifies queries in real-time
- Guides the model's responses more effectively
- Enhances the user's ability to optimize results

This approach essentially turns the AI into an active interviewer that collects precise information before generating its final output.

### Chain-of-Thought Approach

The chain-of-thought approach is a prompt-based learning strategy that guides generative AI models through logical reasoning processes.

- **Task Breakdown** - Breaking complex problems into smaller, more manageable steps through a sequence of straightforward prompts
- **Demonstrated Reasoning** - Providing the model with related questions AND their step-by-step solutions before asking a new question
- **Logical Pattern Recognition** - Training the model to recognize and apply similar reasoning patterns to new problems

#### Example Application:

- **Step 1** - Provide a similar example with solution

        Example Problem: "In a class of 50 students, 40% are boys. After 5 more boys join the class, what percentage of the class is now boys?"

        Example Solution: "In a class of 50 students, 40% are boys. That means there are 0.40 × 50 = 20 boys. After 5 more boys join, there are now 20 + 5 = 25 boys. The total number of students is now 50 + 5 = 55. So the percentage of boys is (25 ÷ 55) × 100 = 45.45%."

- **Step 2** - Present the actual problem

        New Problem: "A store has 80 items, and 25% of them are on sale. If the store adds 20 more sale items, what percentage of the store's items are now on sale?"

There are a few words that, when added to the prompt, are likely to solicit better answers since they invite the AI to do step-by-step reasoning, much like a human would when trying to come to a resolution. According to researchers, two effective phrases are: `Let's think step by step.` and `Let's work this out in a step by step way to be sure we have the right answer.`

Instead of asking a generic question, we can break it down into steps we want the model to consider to develop a much richer and valuable answer. An effective phrase is: `Consider and include the following elements in your answer:`

#### Benefits:

- Strengthens cognitive abilities of AI models
- Encourages step-by-step thinking processes
- Produces more coherent and logically-sound responses
- Helps models understand context and maintain reasoning through conversations

### Tree-of-Thought Approach

The tree-of-thought approach is an innovative technique that expands upon the chain-of-thought prompting method, enabling generative AI models to demonstrate more advanced reasoning capabilities.
This approach essentially creates a simulated "team of experts" within the model, allowing it to explore different solution paths in parallel while maintaining the ability to prune less promising directions.

- **Hierarchical Structure** - Organizing prompts in a tree-like structure to specify desired reasoning paths
- **Multiple Reasoning Paths** - Generating and exploring several lines of thought simultaneously (unlike linear approaches)
- **Branch Evaluation** - Assessing different thought paths and assigning values based on predicted outcomes
- **Path Pruning** - Eliminating less promising lines of thought to focus on the most favorable options
- **Collective Expertise** - Simulating multiple experts collaborating on a problem, each contributing steps in their thinking

#### Example Application:

- **Instruction Format Option 1**:

        "Simulate three brilliant, logical experts collaboratively answering a question. Each one verbosely explains their thought process in real-time, considering the prior explanations of others and openly acknowledging mistakes. At each step, whenever possible, each expert refines and builds upon the thoughts of others, acknowledging their contributions. They continue until there is a definitive answer to the question.The question is..."

- **Instruction Format Option 2**:

        "Identify and behave as three different experts that are appropriate to answering this question.
        All experts will write down the step and their thinking about the step, then share it with the group.
        Then, all experts will go on to the next step, etc.
        At each step all experts will score their peers response between 1 and 5, 1 meaning it is highly unlikely, and 5 meaning it is highly likely.
        If any expert is judged to be wrong at any point then they leave.
        After all experts have provided their analysis, you then analyze all 3 analyses and provide either the consensus solution or your best guess solution.
        The question is...."

- **Original Question**:

        "Bob is in the living room.
        He walks to the kitchen, carrying a cup.
        He puts a ball in the cup and carries the cup to the bedroom.
        He turns the cup upside down, then walks to the garden.
        He puts the cup down in the garden, then walks to the garage.
        Where is the ball?"

#### Benefits:

- Encourages step-by-step logical thinking
- Builds upon intermediate thoughts
- Explores multiple possible solution paths simultaneously
- Allows self-correction when a path proves unproductive
- Maximizes the model's reasoning capabilities
- Produces more comprehensive results by considering various perspectives
- Particularly valuable for complex problem-solving requiring explicit constraints

Dave Hulbert [suggested](https://github.com/dave1010/tree-of-thought-prompting/blob/main/tree-of-thought-prompts.txt) a few rather convincing prompts that leverage this approach and yield, anedotically, great results. I particularly like how he incorporates the Persona pattern and recommend you approach ToT prompting using his prompts or similar variations you might develop yourself.

In a research paper [(i.e., arXiv:2305.10601), Yao et al.](https://arxiv.org/abs/2305.10601) compared various approaches to prompting, including naive prompting, CoT, as well as a new technique called Tree-of-Thought (ToT).

## Module 3

### Core Concept

- Image prompts are text descriptions used to generate images through AI models
- Effective prompting techniques can significantly improve the quality and impact of AI-generated images

### Five Main Prompting Techniques

#### Style Modifiers

- Descriptors that influence artistic style or visual attributes
- Can specify art styles, historical periods, photography techniques, materials, or emulate specific artists/brands
- Helps modify visual elements like color, contrast, texture, shape, and size

#### Quality Boosters

- Terms that enhance visual appeal, fidelity, and sharpness
- Improve specific features resulting in more coherent output
- High-quality images appear more convincing and reliable than low-quality ones

        Examples: "high resolution," "2k," "4k," "hyper-detailed," "sharp focus," "complementary colors"

#### Repetition

- Emphasizes particular visual elements by repeating words or phrases
- Creates familiarity for the model, focusing it on specific ideas
- Helps with abstract or ambiguous prompts by generating multiple variations

        Examples: repeating words like "tiny," "dense," "enormous," "vast," "serene"

#### Weighted Terms

- Words with powerful emotional or psychological impact
- Can assign positive or negative weights to emphasize or de-emphasize certain elements
- Examples: assigning weights to terms like "warm" (+10), "crackling" (+8), or "colorful" (-6)
- Creates images that are more memorable and emotionally resonant

#### Fix Deformed Generations

- Techniques to correct anomalies like distortions, particularly in body parts
- Uses negative prompts to mitigate issues with deformed images
- Helps maintain visual appeal and clarity
