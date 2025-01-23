
---

## ** Prompt Engineering & Frameworks Presentation**

### **Slide 1: Title**
- **Slide Content**: “**Prompt Engineering & Frameworks**”

“Hello everyone, and welcome to my short presentation on **Prompt Engineering** and **Prompt Frameworks**. My name is Javi, and over the next minutes, we’ll explore what prompt engineering is, why it matters, and how specific frameworks can help us get better results from AI models. We’ll also see how we can use a large language model like **Gemini** in both developer and everyday scenarios.”

---

### **Slide 2: What Is Prompt Engineering?**
- **Slide Content**: A definition of prompt engineering, plus reasons why we use prompt frameworks.

“First, let’s define **Prompt Engineering**. Essentially, it’s about creating clear, targeted instructions—known as *prompts*—for large language models. Because models like Gemini, GPT, or Llama 2 interpret our words so literally, writing a well-structured prompt can be the difference between an answer that’s vague or off-topic and one that’s accurate and actionable.  

We use **Prompt Frameworks** because they help us add clarity and consistency. They remind us to include crucial information—like the role the AI should take, the context or constraints, the style or format we want, and the purpose of our request. This makes sure we’re not leaving anything out. Plus, correclty phrasing the prompt can contribute to saving on tokens, potentially reducing costs and time.

AI companies like Google (with their Gemini models) typically charge for usage based on a pay-as-you-go model tied to the number of tokens processed.”

Prompting is more than just typing words into ChatGPT or Google’s Gemini. It’s part creativity—knowing exactly what you need—and part scientific method—testing, refining, and repeating.

---

## **Slide 3 Top Free AI Services**

“Let’s take a look at four AI services that offer free prompting, each with different token limitations and usage policies:

**ChatGPT (Free)**: OpenAI’s popular conversational model, perfect for a variety of tasks. On the free tier, you get about 4,000 tokens per session, which is usually enough for short-to-medium conversations, but watch out for usage caps if you’re sending a lot of requests.

**Microsoft Copilot**: Integrated into Microsoft’s ecosystem, this assistant is handy for everything from writing Word docs to coding in GitHub. It typically handles around 2,048 tokens per request, so it’s great for concise tasks.

**Anthropic’s Claude**: Designed with privacy in mind—helpful for sensitive queries or data. The free tier generally supports about 1,000 tokens per prompt, so you’ll want to keep prompts short and to the point.

**Gemini 1.5 Pro**: Another privacy-focused AI, especially for sensitive data scenarios. The free tier offers 32,000 tokens per minute, which is quite generous. However, you’ll still want to be mindful of how quickly those tokens can add up on more complex tasks.

Using the right prompt framework can help you conserve these precious tokens by crafting more efficient and effective prompts. This ensures you get the most out of your AI interactions, saving both costs and time for when you need them most. If you’re working on a large-scale or complex prompt, consider frameworks like CRISP or TCREI to keep your instructions concise and focused, which helps prevent token overuse.”

---

### **Slide 4: Popular Prompt Frameworks**
- **Slide Content**: A table comparing TCREI (Google recommends), CRISP, SCQA, RTF, Chain-of-Thought (COT), and RASCEF.

“Here we have a table of **popular prompt frameworks**, each with different strengths, weaknesses, and ideal use cases. Let’s go over them briefly:

1. **TCREI (Google recommends)** Iterative approach emphasizing evaluation and references (like code snippets or style guides).
2. **CRISP** focuses on context, role, input, steps, and purpose—great for detailing tech tasks.  
3. **SCQA** is a story-like approach for problem-solving, framing situation → complication → question → answer.  
4. **RTF** stands for role, task, and format—very straightforward, perfect for quick instructions.   
5. **Chain-of-Thought** helps you see the AI’s reasoning—useful for debugging or complex tasks.    
6. **RASCEF** is comprehensive—role, audience, style, context, examples, format—great for formal or multi-stakeholder tasks.

It’s important to pick the right framework for your goal. If you need something short and sweet, **RTF** is awesome. If you need to cover many details, **TCREI** or **CRISP** might be better. If you want to see the AI’s thought process, COT is ideal.”

---

### **Slide 5: Best Practices for Optimal Usage****

“Let’s take a quick look at these **best practices** for making the most of AI in your projects. First, I recommend focusing on complex or high-value tasks—things that really benefit from deeper analysis and creative problem-solving. For coding, consider assigning multiple **roles**—for instance, a coding architect and an engineer—to combine broader design thinking with detail-oriented execution.

It’s also important to **provide comprehensive context**. The more information you supply upfront, the fewer follow-ups you’ll need. Remember, **prompt engineering** is a skill—spend some time learning how to craft your inputs so the AI can give you its best possible output.

Keep in mind that **complex tasks** may require more computation time, so set **realistic expectations** for how long the AI might take. Finally, treat the AI as a **collaborative tool**, not a standalone solution. It’s here to enhance human expertise, not replace it. By balancing clarity in your prompts with an understanding of the model’s capabilities, you’ll see the best results in your workflow.” 

And more thing always verify facts and avoid sharing confidential info. Think of AI as your cool helper, but you, are still the boss!

---

### **Slide 6: Using Gemini**
- **Slide Content**: Explains that we’re importing Gemini and can use these frameworks for various tasks.

“Now, we’ll look at how these frameworks apply in practice. We’ll be using **Gemini**, a large language model by Google, similar to GPT. The steps I’ll show you can also apply to other LLMs since frameworks are **model-agnostic**. It’s all about writing clear prompts and letting the AI handle the rest.  

In our notebook, we have some simple Python code that imports the Gemini client—this is similar to how you might use a library for GPT, Llama, or any other LLM. Let’s see how we actually create prompts for two scenarios: one for **developers** and another for **everyday tasks**.”

---

### **Slide 7: Developer Scenario (CRISP)**
- **Slide Content**: The CRISP-based prompt for a Node.js app returning 500 errors.

“Here’s an example of using **CRISP** in a developer scenario. Suppose we have a Node.js application throwing 500 errors whenever an API key header is missing. Our prompt includes all the relevant pieces: context about the Node app, the role as a *senior backend engineer*, the input code snippet, the steps we want for debugging, and the ultimate purpose—fixing those errors.  

When Gemini sees this, it understands the context, the debugging tasks, and the desired outcome. It can then give us a concise or detailed plan to refactor or fix our middleware to properly return 401, rather than a 500 error.”

---

### **Slide 8: Everyday Scenario (RTF)**
- **Slide Content**: The RTF-based prompt for drafting an apology email.

“Here’s a simple everyday-life scenario. We need to write a quick apology email for a delayed meeting. We use **RTF**—role, task, format. We assign the role of *polite personal assistant*, specify the task—draft an apology email—and define the format—a short, formal paragraph.  

Gemini (or any LLM) takes these instructions and returns a neatly written paragraph. No overcomplicating with steps or context—it’s a straightforward approach, perfect for small, quick tasks.”

---

### **Slide 9 Key Takeaways**
- **Slide Content**: Four bullet points highlighting the importance of prompt engineering and frameworks.

“At this point, let’s recap the **key takeaways**:

1. Prompt engineering is about guiding AI models for **better, more relevant answers**.  
2. Frameworks like CRISP, RTF, SCQA, and others help ensure **clarity and consistency**.  
3. These frameworks are **model-agnostic**—they work with Gemini, GPT, Llama, or any LLM.  
4. **Pick a framework** based on the complexity and context of your task. For short tasks, keep it simple; for complex tasks, provide more detail.”

---

### **Slide 10: Next Steps**
- **Slide Content**: Encourages further experimentation with frameworks, references the Gemini cookbook, and suggests iterative refinement.

“So, where do we go from here?

- **Explore** more frameworks: experiment with SCQA, PEEL, or RASCEF.  
- Check out the [Gemini Cookbook](https://github.com/google-gemini/cookbook) for more advanced examples and best practices.  
- **Iterate and refine**—the more you experiment, the better you’ll understand how to structure prompts for the best results.  

Thank you for joining this quick tour of **Prompt Engineering** and **Frameworks**. I hope you found this introduction helpful, and I encourage you to try out these frameworks in your own projects!”

---

### **End of Presentation**

“That wraps up our presentation. If you have any questions or want to dive deeper into any specific framework, feel free to ask. Thanks for watching!”

---
