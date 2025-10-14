From this discussion, I could see more clearly how Agent Communication Languages (ACLs), such as KQML and FIPA-ACL, give agents a structured way to communicate. Instead of calling methods directly, like in Python or Java, they use performatives such as inform, ask, or request, which come from speech act theory (Searle, 1969). This means agents can understand the intention behind a message rather than just executing a command, something that connects well with what we learned about autonomy in Unit 1 and about reasoning in Units 3 and 4.

Both of my peers agreed that ontology management is one of the main challenges for ACLs. As Payne and Tamma (2014) explain, agents can misunderstand each other if they don’t share the same concepts, which reflects what Unit 6 discussed about communication breakdowns and the need for consistent knowledge representation. Compared with direct method invocation, ACLs are slower but far more flexible. Method calls work well in closed environments where everything is predefined, while ACLs are made for open, dynamic systems where agents decide how to respond (Finin et al., 1994; Wooldridge, 2009).

My colleagues also mentioned new communication protocols such as the Model Context Protocol (MCP), introduced by Anthropic (2024). I agree that MCP is an interesting development because it focuses on connecting agents and tools rather than only agents among themselves. It reminds me of the ideas in Unit 7 about how understanding context improves communication.

Overall, I believe ACLs still play a key role in giving agents the ability to reason and negotiate, while newer protocols like MCP make them more adaptable to modern AI systems that depend on external data and services.

### References

Anthropic (2024) Introducing the Model Context Protocol: An open standard for connecting AI models to tools and data. Available at: https://www.anthropic.com/news/model-context-protocol (Accessed: 5 September 2025).

Finin, T., Fritzson, R., McKay, D. and McEntire, R. (1994) ‘KQML as an agent communication language’, Proceedings of the Third International Conference on Information and Knowledge Management, pp. 456–463. ACM. Available at: https://doi.org/10.1145/191246.191322 (Accessed: 5 September 2025).

Payne, T.R. and Tamma, V. (2014) ‘Negotiating over ontological correspondences with asymmetric and incomplete knowledge’, Proceedings of the International Conference on Autonomous Agents and Multiagent Systems (AAMAS ’14), pp. 517–524. ACM. Available at: https://doi.org/10.5555/2615731.2615816 (Accessed: 5 September 2025).

Searle, J.R. (1969) Speech Acts: An Essay in the Philosophy of Language. Cambridge: Cambridge University Press.

Wooldridge, M. (2009) An Introduction to MultiAgent Systems. 2nd edn. Chichester: John Wiley & Sons.