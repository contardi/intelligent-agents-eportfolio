by Rayyan Mohamed Abdalla Alshambeeli Alnaqbi

Hi Thiago,

Your explanation makes it clear what the main difference is between Agent Communication Languages (ACLs) like KQML and regular method invocation. It focuses on the use of performatives based on speech act theory (Searle, 1969). This semantic richness lets agents talk to each other in a meaningful way without having to know how each other works, which is very important in environments that are distributed and varied (Finin et al., 1994).
I also think it's very important that you talked about the problems that come up with ontology management. Ontology alignment is still a major problem in real-world ACL deployments because semantic mismatches can easily break communication (Payne and Tamma, 2014). The trade-off between efficiency and flexibility that you talk about is the main reason why ACLs are used more in open, dynamic systems and method invocation is used more in closed, tightly coupled systems.

The Model Context Protocol (MCP) is a new standard that connects agents and external tools. This is an interesting development. MCP's role in making it possible for agents and tools to work together shows how AI systems are changing and how important it is for them to be able to access outside context and services (OpenAI, 2024). This protocol works with traditional method calls instead of replacing them. This shows that modern AI architectures use a mix of different ways to communicate.
In general, your post gives a good overview of how ACLs, method invocation, and newer protocols like MCP all have different jobs to do depending on what the system needs.


### References:
Finin, T., Fritzson, R., McKay, D. and McEntire, R. (1994) ‘KQML as an agent communication language’, Proceedings of the Third International Conference on Information and Knowledge Management, pp. 456–463. [Online] Available at: https://doi.org/10.1145/191246.191271 [Accessed 8 Sep. 2025].
OpenAI (2024) ‘Introducing the Model Context Protocol (MCP)’, OpenAI Blog. [Online] Available at: https://openai.com/blog/mcp [Accessed 8 Sep. 2025].
Payne, T. and Tamma, V. (2014) ‘Ontologies for agent communication languages’, Journal of Autonomous Agents and Multi-Agent Systems, 28(2), pp. 213–240. [Online] Available at: https://doi.org/10.1007/s10458-013-9211-7 [Accessed 8 Sep. 2025].
Searle, J.R. (1969) ‘Speech acts: An essay in the philosophy of language’, Cambridge University Press. [Online] Available at: https://doi.org/10.1017/CBO9781139173438 [Accessed 8 Sep. 2025].

--------


by Paul Dogar

Thiago’s post and Rayyan’s response together capture the core distinction between ACLs and method invocation, as well as the evolving role of protocols like MCP. The grounding in speech act theory (Searle, 1969) emphasises how ACLs enable meaningful, intention-driven exchanges, which is vital for heterogeneous environments (Finin et al., 1994). Rayyan rightly stresses the persistent issue of ontology alignment, since mismatched terms can undermine communication and coordination (Payne and Tamma, 2014).

What stands out in both contributions is the recognition that MCP occupies a different but complementary layer. Unlike ACLs, which focus on inter-agent semantics, MCP offers a universal interface for connecting agents with external tools and services (OpenAI, 2024). This suggests that modern systems benefit most from hybrid strategies: ACLs for negotiation and reasoning, MCP for tool interoperability, and method invocation for efficiency in tightly coupled environments. Together, these form a layered architecture rather than competing paradigms.

### References

Finin, T., Fritzson, R., McKay, D. and McEntire, R. (1994) ‘KQML as an agent communication language’, Proceedings of the Third International Conference on Information and Knowledge Management, pp. 456–463. ACM. Available at: https://doi.org/10.1145/191246.191322 (Accessed: 11 September 2025).

OpenAI (2024) Introducing the Model Context Protocol (MCP). Available at: https://openai.com/blog/mcp (Accessed: 11 September 2025).

Payne, T.R. and Tamma, V. (2014) ‘Negotiating over ontological correspondences with asymmetric and incomplete knowledge’, Proceedings of the International Conference on Autonomous Agents and Multiagent Systems (AAMAS ’14), pp. 517–524. ACM. Available at: https://doi.org/10.5555/2615731.2615816 (Accessed: 11 September 2025).

Searle, J.R. (1969) Speech acts: An essay in the philosophy of language. Cambridge: Cambridge University Press.

