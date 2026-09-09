A concise overview of automating systems management:

### Introduction
- Motivate the need for automated systems management


### The Design
- Introduce the design and explain its structure.
- Frame the design as a closed semantic world with established narratives.
- Explain that the closed semantic world can be reasoned about given that the design establishes the necessary meaning
- Explain how reasoning about the world does the following:
   - Failure prediction and resolution using invariants
        - Semantic invalidity is when the world state means the designs intentions can't be realized.
        - Environment must have a semantically valid path through the design
   - Testing
        - Test that semantically invalid narratives are not possible
   - Failure Diagnosis
        - Test that design respects all known invariants
        - Failure only means new semantics must be learnt
   - Debugging
        - Which invariant was violated?
- Explain how any form of reasoning is possible given that the necessary meaning has been established
- Explain how if the design is represented in an unambiguous and structured form, an engine can automatically reason about the entire world
- This would automate all forms of reasoning mentioned earlier


### Semantic Reasoning Engine
- Explain how the design can be written in the Design Abstraction Language
    - The scope of the language is any mechanism needed to represent the designs meaning faithfully
- Explain how an engine can reason about the closed semantic world
    - DAL script is an input into the engine
- Explain how these two together would automate the reasoning of the world
    - Engine would automatically answer the question given the necessary meaning has been established


### Computable Semantic Model
- Software Systems are the result of an intentional design
- Programming languages are used to realize the meaning of the design
- If the semantic gap between the design and the implementation is eliminated, then the design can be used to reason about the software system
- This would enable automated systems management and it would inherit all the automation enabled by the design and engine
- This is achieved by establishing semantic primitives that are used to construct the closed semantic world and synthesize and executable implementation of the designs meaning
- The execution literally realizes the meaning of the design
- This closes the semantic gap and enables automated systems management


### Automated Systems Management
- Using the CSM built from CSP's, the software system can be entirely reasoned about using the engine
- This means that the management of software systems can be fully automated because any meaningful question that is asked about the design can be answered by the engine given that the necessary meaning has been established
- As part of the automated management, a learning loop emerges where the design learns new semantics through root cause analysis on environments that caused the failure
- The learning loop for failures is just one part of systems management, there are many scenarios in which abnormal behavior is managed
- Ultimately, any question that cannot be answered results in semantics being expanded through root cause analysis  
- However, practically, this would require all the environments to be preserved
- To address this, the designs unambiguous nature is exploited to log non-reproducible information and to apply domain specific compression to the environments to preserve them losslessly at minimal cost
- Compressed Log Processor is a tool that can be leveraged to address this problem, it has been proven at a petabyte scale.
- The CSM eliminates ambiguity in the construction of software systems and CLP maximizes its compression through the unambiguous construction.
- This will transform CLP into a domain specific compression engine, where the domain of the data is specified and CLP compresses it.
- Together, CSM, CLP and the engine automate the management of software systems at scale.


### Design Learning Platform
- Practical system that realizes this solution.
- Present system diagram.
- The engine reasons abut the world, eliminates failures and then instruments the execution with the information it needs to learn from failures
- The engine also answers any arbitrary question about the world to manage it
- CLP preserves all the environments
- Engine also reasons about the world in other ways, the only limitation is the meaning that is encoded
- Since the meaning of the system and its state is unambiguous, the orchestration can surgically manage the system to recovery from failures and perform life cycle operations
- Practically, this entire process will result in a design repository that can deterministically replay the evolution of the design


### Implications
- Software system development is now about world building
- The world has unambiguous meaning and intention
- Distributed systems are simply semantically compatible interactions between designs (or closed semantic worlds), building a larger closed semantic world
- The same way that designs can be reasoned about, can be extended to distributed systems
- All the automation is inherited at that level
- Systems that operate at this level of meaning are more secure
- This way of building software systems will open the door for many new opportunities


### Conclusion
- CSM is logical conclusion of software development process
- CLP is novel solution that address unknown that prevented automated systems management
- Engine is simply processing the design
- Conclude by explaining how this addresses the goals laid out at the start