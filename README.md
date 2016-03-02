# PEDSEWAN
Platform for Evaluating Distributed Systems on Emulated Wide-Area Networks

The evaluation of distributed system could be done by simulating relevant system aspects or by executing the system in real deployment environments. Simulation works well for particular system aspects, but covering all implications from the components' interactions is a much more difficult task. The execution in the real deployment environment on the other hand has its own drawbacks. Besides the fact that real hardware may cause high costs the main disadvantage is that the changing environmental conditions make it impossible to obtain deterministic results. 

Therefore PEDSEWAN chooses the way of emulation as it combines the advantages of both approaches. The unmodified system can be executed in an environment that allows the emulation of any host specific condition as well as the conditions of the execution environment - resulting in reproducible results. But emulation also comes with high setup and bootstrapping efforts which in most cases exceed those from simulation or real deployments as it requires both a real deployment and the modelling of certain aspects. PEDSEWAN gets ride of those drawback by providing a comprehensive automation strategy.

To reach those goals PEDSEWAN controls every aspect of the experiment livecycle. It connects to existing infrastructure provisioning services to allocate the required execution nodes. It controls the conditions of the nodes using agents located on those nodes and the conditions of the interconnecting network by routing all traffic through a dedicated traffic shaper node. The experiment execution is completely automated by the platform. All actions are executed according to the defined schedule, before the experiments reports are collected and all utilized resources are released and cleaned up.

We are currently still working on the first prototype which will be released here at the beginning of April 2016. So stay tuned…
