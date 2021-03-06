- three types of relations between processes
	- independent processes (no communication or synchronization)
		- if a process fails, no influence on other processes
		- reliability achieved through use of [[recovery blocks (dynamic software redundancy)]] + handling exceptions
	- cooperating processes (communication and/or synchronization)
		- if a process fails, influence on other processes, introducing [[atomic action]]
	- processes in competition of resources 
		- synchronization of resources, deal in [[Chapter 08 Resource control]] 
- [[atomic action]] and [[atomic transaction]]
- [[language support of atomic action]] (chapter 7.2, must study)
	- [[atomic action]] in Java: similar to C, but instead of using conditional variables, Java use guard. 
	- [[atomic action]] in C/POSIX: 
	- [[atomic action]] in Ada: Code example at [[code.Z.handbook.235]]. 
- [[atomic action]] can be used in [[backward recovery]] during concurrent tasks if error appears inside the [[atomic action]]
- [[asynchronous events]], signals and asynchronous transfer of control
	- [[signals in POSIX]]
	-  asynchronous transfer of control in Ada/Java (use [[termination model]])