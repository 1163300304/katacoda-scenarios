We design and implement a Linux kernel static analysis system based on 
LLVM. The system can use PeX based indirect call analysis technology to build a 
complete function call graph, find out all suspicious bug paths, and use the symbolic 
execution engine based on Deadline and KUBO to verify these paths one by one.The 
system is generally applicable to the verification of possible trigger paths of different 
kinds of bugs in the kernel, and it is modular design so taht each analysis function can 
be relatively independent. This paper also uses the system to analyze the kernel, verify 
the PeX outputing permission check bugs, and comprehensively evaluates the system.
After testing, the efficiency of the system reaches 100 paths per second, and test 
coverage rate for path reaches 92%.

## Task

We have customized the necessary environment, including nodejs.

`node -v`{{execute}}


We draw on the achievements of Kubo `katacoda-scenario-examples/create-scenario-101/KUBO Precise and Scalable Detection of User-triggerable.pdf`{{open}}

The JSON file defines the scenario title, the description, steps order, the UI layout and environment. You can find more about the system within our scenarios at [katacoda.com/docs/scenarios/layouts](https://katacoda.com/docs/scenarios/layouts) and environments at [katacoda.com/docs/scenarios/environments](https://katacoda.com/docs/scenarios/environments).
