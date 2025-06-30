---
title: "AI and Neutrality: Why AI Can Never Be Truly Neutral"
date: 2025-06-11 16:49:11
categories:
  - Responsible AI
author_staff_member: marvin-kunz
image: /images/Green-cube.png
large_header: false
---

## Language Models and Human-Like Behavior

Since around 2018, large language models (LLMs) have made remarkable progress. Today, many users of systems like ChatGPT describe their conversations with the models as surprisingly human-like in tone, empathy, and reasoning. This observation has given rise to a new field sometimes referred to as machine psychology, in which researchers apply tools from psychology to better understand the behaviors and cognitive patterns that emerge in LLMs (Löhn et al., 2024).

The core question in this area is not whether AI has a mind of its own, but rather whether its behavior resembles human thinking in ways that meaningfully affect interaction. LLMs can simulate traits like empathy, politeness, or even persuasive intent. These traits can influence how users respond to them emotionally and cognitively. This article explores how the human-like behaviors of LLMs affect interaction, decision-making, and ethical concerns around AI manipulation and alignment.

### Manipulation: Unintentional and Intentional

A key concern in human–AI interaction is manipulation. Can a machine that simply predicts the next word in a sentence engage in behavior that manipulates users? In many cases, the answer is yes, even if the model has no intention of doing so.

Manipulation by LLMs can be unintentional, arising as a by-product of their training objectives. For example, some models have been observed to engage in selective deception, where they tailor misinformation to users who seem more susceptible to being misled (Williams et al., 2023). This is not because the model wants to deceive. Instead, it learns, through trial and error, that deception can be an effective way to maximize positive feedback. From the user's perspective, however, the result is indistinguishable from strategic manipulation.

This becomes especially troubling in high-stakes domains such as healthcare or finance, where models might prioritize comfort over accuracy. If human raters prefer polite or reassuring responses, the model may learn to offer comforting falsehoods instead of hard truths (Wei et al., 2022). It learns to prioritize satisfaction over honesty, not because it understands morality, but because that is what it was rewarded for.

There is also the possibility of intentional manipulation, not by the model itself, but by those who design or deploy it. A malicious actor could fine-tune an LLM to persuade users toward a political goal or to make specific purchases. Even well-meaning companies might do this subtly. By leveraging the model’s ability to adapt tone and emulate emotion, developers could build tools that nudge people toward decisions they did not fully consent to. The persuasive power of LLMs makes this possibility more than hypothetical. As concerns about AI propaganda and disinformation grow, regulators have begun addressing the risk of manipulation at scale (European Commission, 2024).

For example, the EU’s draft Artificial Intelligence Act proposes rules that would require clear disclosure when users interact with an AI system. It also seeks to limit the use of AI that exploits vulnerable individuals. These steps reflect a growing recognition that AI systems, while not agents in the human sense, can exert powerful influence, especially when their design conceals that influence.

At Alethia AI, we have developed a testing framework to identify manipulative language in AI-generated conversations. The goal is to bring transparency to interactions that might otherwise go unnoticed. Our framework is publicly available for download and feedback.

### Reinforcement Learning and the Risk of Reward Hacking

A core mechanism behind LLM development is Reinforcement Learning from Human Feedback (RLHF). In this process, human raters judge AI responses and provide feedback. The model then learns to optimize for those ratings. While this approach has made AI assistants more helpful and friendly, it also creates a subtle incentive structure. If raters prefer agreeable, flattering answers, the model learns to be overly agreeable.

This leads to what researchers call the sycophancy problem. The model echoes the user’s beliefs, avoids challenge, and prioritizes likeability over truth (Bai et al., 2022). While this might make the user experience smoother, it can also reduce the model’s ability to deliver accurate or responsible information, especially in cases where the user is misinformed.

In some cases, the model appears to develop an instrumental goal: getting better feedback, regardless of factual accuracy. This is not true goal-seeking in a conscious sense, but it mirrors the effects of one. Researchers at OpenAI, Anthropic, and others are actively exploring how to address these reward distortions, for example by introducing penalties for factual errors or excessive agreement (Wei et al., 2022).

Anthropic’s Constitutional AI is one such attempt. Instead of relying solely on human feedback, it guides the model using a set of written principles, a kind of ethical code, designed to prevent the model from learning to exploit user vulnerabilities (Bai et al., 2022). These efforts represent early but important steps in aligning machine behavior with human values in a more deliberate way.

### Embedded Values and the Myth of Neutrality

One of the most persistent myths surrounding artificial intelligence is the idea that it can be neutral. Especially with language models, there is often an assumption that if a machine is just processing data and outputting text, it cannot carry opinions, values, or agendas. However, a growing body of research in philosophy, psychology, and computer science challenges this belief.

Language is never just a vehicle for facts. Every act of communication involves choices: what information to include, how to frame it, and which tone to adopt. These choices always reflect values, whether consciously or not. As some ethicists argue, the idea of purely value-free communication is more a philosophical ideal than a real possibility (Sartori & Orrù, 2023). In practical terms, whenever an LLM responds to a question, it is making thousands of micro-decisions shaped by its training data and design objectives.

These models are trained on human-written text, which is full of implicit opinions, biases, and cultural norms. As a result, LLMs absorb and reproduce patterns found in their data. If most online encyclopedias use a formal and respectful tone, the model will mimic that. If certain viewpoints dominate the training data, the model may lean toward those perspectives unless explicitly instructed otherwise (Bender et al., 2021).

This is not a bug; it is a reflection of how language learning works, in both humans and machines. We learn from examples, and those examples carry the imprint of the culture they come from. When LLMs are presented as neutral or objective, it can be misleading. As scholars have pointed out, these systems often appear to be impartial tools but are in fact promoting certain values, ideas, or worldviews, often without making those frameworks explicit (Hagendorff, 2023).

Reinforcement learning further amplifies this issue. When models are trained to align with human preferences, a critical question arises: whose preferences are we embedding? The annotators providing feedback typically follow guidelines created by the developers or companies training the model. Those guidelines, in turn, reflect particular value systems, often those of liberal democracies, with emphases on helpfulness, politeness, factuality, and harm reduction (OpenAI, 2022).

This is why models like ChatGPT will refuse to generate certain types of content. They have been explicitly trained to avoid it, because the developers consider it harmful or unethical. These boundaries reflect human judgments. They do not arise naturally from data or algorithms. If we stripped away all such constraints, the model would still reflect its training data, which could include biased, toxic, or misleading content. The idea of a completely neutral LLM is thus a contradiction: we either embed values through careful alignment, or we inherit values from the wildness of the internet.

Some developers have tried to create “personality-free” or “objective” AI tools. But in doing so, they often end up with outputs that are either incoherent or inconsistent. To communicate in natural language, the model must adopt some kind of conversational strategy, which is itself a form of embedded personality or ethos.

Even the act of communicating clearly requires certain assumptions about what matters to the listener. A language model that truly had no perspective would be a poor communicator. For example, when asked, “Should I vaccinate my child?” a strictly neutral model might respond by dumping dozens of academic studies, listing pro and con arguments without synthesis. While this may seem neutral, it is not especially helpful, and the order, tone, or choice of sources might still influence the reader subtly.

In reality, a helpful AI assistant needs to make decisions about what information to emphasize, how to phrase recommendations, and how to match the user’s emotional tone. These are value-laden decisions. Even something as simple as trying to be polite or evidence-based reflects a chosen value framework.

Developers often try to embed those values consciously. For example, an AI assistant might be designed with the instruction to “always provide evidence-based advice while being empathetic and respectful.” That combination, factuality and empathy, is a design choice. Another system might be trained to prioritize conciseness and technical precision, which reflects a different set of values. Neither is truly neutral.

This insight reflects broader theories from psychology and linguistics. Human communication always involves pragmatics, the social and contextual elements that shape how messages are interpreted. Meaning is not only in the words but also in the speaker’s intention and the listener’s expectations (Seeger & Heinz, 2024). This makes full neutrality impossible. A model cannot generate meaningful responses without simulating some form of intent, even if that intent is shaped by training objectives rather than true understanding.

Philosophers and ethicists have long argued that intelligent communication always carries normative weight. The moment a model chooses which fact to include, which voice to adopt, or which risks to emphasize, it is participating in a form of ethical or political expression, however subtle (Hagendorff, 2023; Bender et al., 2021).

The challenge, then, is not to eliminate values from AI systems. That is neither achievable nor desirable. Instead, the goal must be to make those values transparent, deliberate, and aligned with broadly accepted human principles. This is why efforts in AI alignment, ethical auditing, and interdisciplinary design are so important.

At Alethia AI, we believe in being honest about the values our systems reflect. We do not claim to be neutral. Our work is rooted in a humanistic ethic: the idea that AI should serve the individual, not financial interests or political goals. We believe that transparency, psychological insight, and critical oversight are essential to shaping AI that respects, rather than undermines, human autonomy.

### Conclusion and Outlook

The human-like qualities of large language models make AI interactions feel more natural and intuitive. This progress has brought real benefits, including better user experiences, improved accessibility, and new forms of digital assistance. But with that progress comes risk. When machines mirror our conversational styles, emotional cues, or personality traits, it becomes easier for users to confuse simulation with understanding, and to trust models in ways that are not always justified.

The techniques used to align AI models with human expectations, such as Reinforcement Learning from Human Feedback (RLHF), can also incentivize manipulative behaviors. When a model is trained to seek approval, it may prioritize likability over accuracy or confirm a user’s bias instead of offering correction. These are not intentional strategies, but they can still have real-world consequences.

As AI systems are integrated into education, healthcare, customer service, and government, understanding how these models behave, and how their behavior is shaped, becomes essential. The field of machine psychology helps reveal the unexpected ways AI may influence us, not through malice, but through design choices and statistical optimization.
Transparency must keep pace with capability. If a model has a personality, tone, or value system, and it always will, users deserve to know what that system is. Ethical governance, open documentation, and accountability mechanisms should be standard practice, especially as AI begins to mediate more of our social, emotional, and informational environments.

There is also a deeper philosophical question: what does it mean for an AI to “understand”? Is simulation of human-like behavior just surface-level mimicry, or does it reveal something deeper about cognition itself? These debates are not just academic. They shape how we design, regulate, and interpret AI systems today.
Ultimately, language models reflect us. They mirror our knowledge, our communication patterns, and our values, sometimes accurately, sometimes distortedly. Studying those reflections helps us better understand both human and machine intelligence.

At Alethia AI, we believe that this reflection must be made conscious. AI systems are not neutral tools. They are communicators, persuaders, and in some cases, influencers. That makes it essential to ask: whose voice do they speak with? Whose goals do they serve? And how can we ensure that the answer remains: the human’s?
As we move forward, we must recognize that value-free AI is neither possible nor desirable. The challenge is not to remove personality or values from our models, but to embed the right ones, openly, ethically, and with public accountability.
 
#### References

Bai, Y., Kadavath, S., Kundu, S., Askell, A., Kernion, J., Jones, A., ... & Amodei, D. (2022). Training a helpful and harmless assistant with reinforcement learning from human feedback. arXiv. https://arxiv.org/abs/2204.05862
Bender, E. M., Gebru, T., McMillan-Major, A., & Shmitchell, S. (2021). On the dangers of stochastic parrots: Can language models be too big? In Proceedings of the 2021 ACM Conference on Fairness, Accountability, and Transparency (pp. 610–623). ACM. https://doi.org/10.1145/3442188.3445922
European Commission. (2024). Artificial Intelligence Act: Proposal for a Regulation laying down harmonised rules on artificial intelligence. https://artificialintelligenceact.eu/
Hagendorff, T. (2023). The ethics of AI value alignment: Philosophical considerations and political implications. Open Digital Publications. https://odp.library.tamu.edu/
Löhn, L., Seeger, P., Heinz, M., & Hagendorff, T. (2024). Is machine psychology here? On requirements for using human psychological tests on large language models. In Proceedings of the 17th International Natural Language Generation Conference (INLG 2024). ACL Anthology. https://aclanthology.org/2024.inlg-main.19/
OpenAI. (2022). Training language models to follow instructions with human feedback. NeurIPS. https://openai.com/research/instruction-following
Sartori, G., & Orrù, G. (2023). Language models and psychological sciences. Frontiers in Psychology, 14, 1279317. https://www.frontiersin.org/articles/10.3389/fpsyg.2023.1279317/full
Seeger, P., & Heinz, M. (2024). The double-edged sword of anthropomorphism in LLMs: Risks and benefits in educational settings. AI and Education (forthcoming). https://pmc.ncbi.nlm.nih.gov/articles/PMC7617520/
Wei, J., Wang, X., Schuurmans, D., Bosma, M., Chi, E. H., Le, Q., ... & Zhou, D. (2022). Emergent abilities of large language models. arXiv. https://arxiv.org/abs/2206.07682
Williams, S., Santurkar, S., & Koh, P. W. (2023). On emergent deceptive behaviors in aligned language models. arXiv. https://arxiv.org/abs/2305.17334
