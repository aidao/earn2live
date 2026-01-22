- 前端开发AI Agent智能体 https://mp.weixin.qq.com/s/wylewnVxyJzeGkQqdCiLqg
- 不写代码、不花钱, 如何利用智能体与MCP 实现UI前端开发 https://mp.weixin.qq.com/s/EplHjVbG9kSTDVgc858MLw
- 智能体（AI Agent）开发完整指南 https://mp.weixin.qq.com/s/40uJUP9oO8ARNuZYT0jKCg
- 前端开发AI Agent智能体，需要掌握哪些知识？https://mp.weixin.qq.com/s/uBS0OHZPd6_Pp48dMYGXVQ
- 从需求到研发全自动：如何基于Multi-Agent架构打造AI前端工程师 https://mp.weixin.qq.com/s/Huf3rfXM0hDqRe87VXiftg
- AI代理的上下文工程：构建Manus的经验教训 https://manus.im/zh-cn/blog/Context-Engineering-for-AI-Agents-Lessons-from-Building-Manus
- Google放大招：让前端工程师也能开发AI智能体了 https://mp.weixin.qq.com/s/IkDF57EWQxbjKIx4w-nR1g
- Solace: Getting started with Agentic ai https://solace.com/blog/getting-started-with-agentic-ai
- https://www.reddit.com/r/ClaudeAI/comments/1ltsxg0/thanks_to_multi_agents_a_turning_point_in_the/
- The Evolution and History of AI Agents https://www.ema.co/additional-blogs/addition-blogs/history-evolution-ai-agents
- https://inspira.ai/agents/history-of-agents-and-agentic-workflows
- https://medium.com/google-cloud/what-is-an-agent-and-does-your-data-need-one-928db7cbde81
- https://www.mindset.ai/blogs/what-is-the-future-of-agentic-ai
- https://www.mindset.ai/blogs/how-have-ai-agents-evolved-over-time
- https://medium.com/google-cloud/what-is-an-agent-and-does-your-data-need-one-928db7cbde81
- Trae官方的 8 个AI 智能体 https://mp.weixin.qq.com/s/Z0fi-ngXUKMcxcwWwUPrhg
- AI Agent（智能体）技术白皮书 https://www.kaggle.com/whitepaper-agents
- AI Agent（智能体）技术白皮书 https://arthurchiao.art/blog/ai-agent-white-paper-zh/

## Agentic AI Development Architecture
```mermaid
graph TB
    Input([Jira/Figma]) --> Manager[Orchestrator Agent]
    Manager <--> Memory[(Shared State & RAG)]
    subgraph P1 [1. Analysis Phase]
        direction TB
        BAA[Business Analyst Agent]
        BAA --- B1[<b>Skills:</b> Requirement Decomp, Story Mapping]
        BAA --- B2[<b>Tools:</b> Jira API, Figma Vision, Confluence]
    end
    subgraph P2 [2. Architecture Phase]
        direction TB
        ARA[Architect & Review Agent]
        ARA --- A1[<b>Skills:</b> Dependency Mapping, Security Auditing]
        ARA --- A2[<b>Tools:</b> Vector Codebase, Mermaid, SonarQube]
    end
    subgraph P3 [3. Development Phase]
        direction TB
        FEA[Frontend Agent: Angular]
        FEA --- F1[<b>Skills:</b> Signals, RxJS, CSS Fidelity]
        FEA --- F2[<b>Tools:</b> Angular CLI, Vitest, Tailwind]
        
        BEA[Backend Agent: Java]
        BEA --- BE1[<b>Skills:</b> SQL Dialect, Spring Security]
        BE1 --- BE2[<b>Tools:</b> Maven, Tools4AI, Oracle/Postgres]
    end
    subgraph P4 [4. QA & DevOps Phase]
        direction TB
        TQA[Testing & QA Agent]
        TQA --- T1[<b>Skills:</b> Self-Healing E2E, Mutation Test]
        TQA --- T2[<b>Tools:</b> Playwright, JUnit 5, JaCoCo]
        
        DOA[DevOps & SRE Agent]
        DOA --- D1[<b>Skills:</b> Pipeline Auto-Fix, Log Triage]
        D1 --- D2[<b>Tools:</b> CircleCI, Jenkins, K8s Lens]
    end
    Manager --> P1
    P1 --> P2
    P2 --> P3
    P3 --> P4
```
