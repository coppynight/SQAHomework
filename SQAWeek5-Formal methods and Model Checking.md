Formal Method and Model Checking
                                                             13126152  XiaoKai
###Formal Method
	Introduction
Formal methods: state of the art and future directions.

Formal methods are techniques used to model complex systems as mathematical entities. By building a mathematically rigorous model of a complex system, it is possible to verify the system's properties in a more thorough fashion than empirical testing.

Formal methods are system design techniques that use rigorously specified mathematical models to build software and hardware systems. In contrast to other design systems, formal methods use mathematical proof as a complement to system testing in order to ensure correct behaviour. As systems become more complicated, and safety becomes a more important issue, the formal approach to system design offers another level of insurance.

Formal methods differ from other design systems through the use of formal verification schemes, the basic principles of the system must be proven correct before they are accepted [Bowen93]. Traditional system design has used extensive testing to verify behavior, but testing is capable of only finite conclusions. Dijkstra and others have demonstrated that tests can only show the situations where a system won't fail, but cannot say anything about the behavior of the system outside of the testing scenarios [Bentley89]. In contrast, once a theorem is proven true it remains true.

It is very important to note that formal verification does not obviate the need for testing [Bowen95]. Formal verification cannot fix bad assumptions in the design, but it can help identify errors in reasoning which would otherwise be left unverified. In several cases, engineers have reported finding flaws in systems once they reviewed their designs formally [Kling95].

Roughly speaking, formal design can be seen as a three step process, following the outline given here:

Formal Specification: During the formal specification phase, the engineer rigorously defines a system using a modeling language. Modeling languages are fixed grammars which allow users to model complex structures out of predefined types. This process of formal specification is similar to the process of converting a word problem into algebraic notation.
In many ways, this step of the formal design process is similar to the formal software engineering technique developed by Rumbaugh, Booch and others. At the minimum, both techniques help engineers to clearly define their problems, goals and solutions. However, formal modeling languages are more rigorously defined: in a formal grammar, there is a distinction between WFFs (well-formed formulas) and non-WFFs (syntactically incorrect statements). Even at this stage, the distinction between WFF and non-WFF can help to specify the design. Several engineers who have used formal specifications say that the clarity that this stage produces is a benefit in itself [Kling95].

Verification: As stated above, formal methods differ from other specification systems by their heavy emphasis on provability and correctness. By building a system using a formal specification, the designer is actually developing a set of theorems about his system. By proving these theorems correct, the formal
Verification is a difficult process, largely because even the simplest system has several dozen theorems, each of which has to be proven. Even a traditional mathematical proof is a complex affair, Wiles' proof of Fermat's Last Theorem, for example, took several years after its announcement to be completed. Given the demands of complexity and Moore's law, almost all formal systems use an automated theorem proving tool of some form. These tools can prove simple theorems, verify the semantics of theorems, and provide assistance for verifying more complicated proofs.

Implementation: Once the model has been specified and verified, it is implemented by converting the specification into code. As the difference between software and hardware design grows narrower, formal methods for developing embedded systems have been developed. LARCH, for example, has a VHDL implementation. Similarly, hardware systems such as the VIPER and AAMP5 processors have been developed using formal approaches.
An alternative to this approach is the lightweight approach to formal design. In a lightweight design, formal methods are applied sparingly to a system. This approach offers the benefits of formal specification, but also avoids some of the difficulties.

###Model Checking
	Introduction
Model checking is a technique for verifying finite state concurrent systems such as sequential circuit designs and communication protocols. It has a number of advantages over traditional approaches that are based on simulation, testing, and deductive reasoning. In particular, model checking is automatic and usually quite fast. 

Also, if the design contains an error, model checking will produce a counterexample that can be used to pinpoint the source of the error. The method, which was awarded the 1998 ACM Paris Kanellakis Award for Theory and Practice, has been used successfully in practice to verify real industrial designs, and companies are beginning to market commercial model checkers.The main challenge in model checking is dealing with the state space explosion problem. This problem occurs in systems with many components that can interact with each other or systems with data structures that can assume many different values. 

In such cases the number of global states can be enormous. Researchers have made considerable progress on this problem over the last ten years.This is the first comprehensive presentation of the theory and practice of model checking. The book, which includes basic as well as state-of-the-art techniques, algorithms, and tools, can be used both as an introduction to the subject and as a reference for researchers.
