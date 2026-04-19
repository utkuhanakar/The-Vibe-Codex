# 📐 System Design & Architecture Prompts

When building large-scale applications—whether it's a web backend or a complex game engine—asking an AI to simply "write the code" leads to brittle, decoupled scripts. 

The secret to "Vibe Coding" at a professional level is forcing the AI to act as a **System Architect** first.

## 🛑 The Mistake: The "Do It" Prompt
> "Write a user authentication system in Node.js."
*Result:* The AI will give you generic boilerplate. It won't ask about your database, session management, or security constraints.

## 💡 The Solution: The "Architect's Constraint" Prompt

Use this template *before* any code is generated. Paste this into Claude or GPT-4 when starting a new module.

### 📝 The Master Architecture Prompt

```text
Act as a Senior System Architect. I am building a [Insert Project Type, e.g., Multiplayer Co-op Game / Full-Stack Web App]. 

Before we write any code, we need to design the architecture for the [Insert Feature, e.g., Inventory System / Payment Gateway].

Here are my hard constraints:
1. Tech Stack: [e.g., Unity & C# / React & Node.js]
2. Data Flow: It must interact with [Insert existing system, e.g., SaveManager / PostgreSQL Database].
3. Performance: It must be highly optimized for [e.g., Network synchronization / High read operations].

Your Task:
1. Do NOT write the implementation code yet.
2. Outline the class/component structures and how they communicate.
3. Identify potential bottlenecks or logic conflicts (e.g., race conditions).
4. Provide a step-by-step implementation plan.

Awaiting your architectural breakdown.
