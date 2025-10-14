by Ana-Maria Stoica 

Agents are computer systems that are capable of acting autonomously to achieve their design objectives in the environment in which they are present. This autonomy sits at the core of agency, enabling the systems to perceive their environment, react to changes, and pursue their goal proactively. A key difference from objects in object-oriented programming (OOP) is that agents maintain control over whether or not they execute actions (Wooldridge, 2009). Multiagent systems are composed of several interacting agents, which can cooperate and coordinate, and ultimately make decisions, all with the purpose of achieving their goals (Drasko and Rakic, 2024).

The critical component of multiagent systems is communication. Various types of systems exist, including non-ACL ones, which are only focused on transmitting information, but agent communication languages (ACLs) such as KQML and FIPA ACL are based on speech acts (Austin, 1962; Suguri, 1999). This enables agents to have complex interactions like negotiations and agreements. Unlike method invocation in Java or Python, where a public method must execute when called, ACLs send requests. Based on these, the receiving agent can choose to act or not, giving them autonomy over their behaviour (Wooldridge, 2009). 

KQML is more lightweight and flexible, making it suitable for simpler communication, and FIPA ACL provides better support for rich semantics and dynamic collaborations, making it suited for environments such as smart cities or autonomous robotics (Drasko and Rakic, 2024). There are of course some disadvantages to these languages, for example KQML is lacking in standardisation, leading to inconsistencies across implementations (Gatti et al, 2025) and alongside FIPA ACL it is seen as rigid and lacking flexibility in the broader sense. Despite these limitations, ACL-based systems are extremely valuable for situations that require coordinated agent interactions, and these issues can very well be solved by improving on existing protocols, making them more adaptable (Drasko and Rakic, 2024).

### References
Austin, J. L. (1962) ‘How to Do Things with Words’, Oxford University Press. Available at: https://doi.org/10.1093/acprof:oso/9780198245537.001.0001 (Accessed: 2 September 2025)

Drasko, B. and Rakic, K. (2024) ‘Analysis of Communication Protocols in Multi-Agent Systems’, DAAAM International Scientific Book 2024 (08), pp. 103–116. Available at: https://doi.org/10.2507/daaam.scibook.2024.08 (Accessed: 2 September 2025)

Gatti, A., Mascardi, V. and Ferrando, A. (2025) ‘ChatBDI: Think BDI, Talk LLM’, Proceedings of the 24th International Conference on Autonomous Agents and Multiagent Systems (AAMAS 2025), Detroit, MI, USA, pp. 2541–2543. Available at: https://doi.org/10.5555/3709347.3743930 (Accessed: 3 September 2025)

Suguri, H. (1999) ‘A standardization effort for agent technologies: The Foundation for Intelligent Physical Agents and its activities’, Proceedings of the 32nd Annual Hawaii International Conference on Systems Sciences. HICSS-32, pp. 10. Available at: https://doi.org/10.1109/HICSS.1999.773093 (Accessed: 3 September 2025)

Wooldridge, M. (2009) ‘An Introduction to MultiAgent Systems (2nd edn.)’, Wiley. Available at: https://www.cs.ox.ac.uk/people/michael.wooldridge/pubs/imas.html (Accessed: 2 September 2025)

### Peer Response
Thank you for a very clear and engaging explanation of how ACLs differ from method invocation. I particularly liked how you highlighted the autonomy aspect, that agents can decide whether to act on a message, unlike in object-oriented method calls, where execution is mandatory. This point really shows why ACLs are better suited to dynamic and unpredictable environments.

I also agree with your contrast between KQML and FIPA ACL. Your point about FIPA ACL being practical in more complex domains like smart cities and robotics makes me think of how crucial semantic richness is when agents need to coordinate in safety-critical systems. At the same time, the lack of standardisation you mention is still a challenge. Payne and Tamma (2014) also emphasised that even with standards like FIPA ACL, semantic mismatches can disrupt communication, which shows that the issue is not only technical but also conceptual.

One additional point I would like to highlight is the role of newer protocols, such as MCP (Model Context Protocol). While ACLs focus on agent-to-agent semantics, MCP provides a standard way for agents, particularly AI models, to connect with external tools and data (Anthropic, 2024). I see this as a different layer of communication that could work alongside ACLs rather than replacing them. It might be a promising way to address the rigidity you mentioned by combining semantic clarity with practical interoperability.

### References
Anthropic (2024) Introducing the Model Context Protocol: An open standard for connecting AI models to tools and data. Available at: https://www.anthropic.com/news/model-context-protocol (Accessed: 5 September 2025).

Payne, T.R. and Tamma, V., 2014. Negotiating over ontological correspondences with asymmetric and incomplete knowledge. In: Proceedings of the International Conference on Autonomous Agents and Multiagent Systems (AAMAS ’14), AAMAS’14, pp. 517–524. ACM. Available at: https://doi.org/10.5555/2615731.2615816 (Accessed: 5 September 2025).
