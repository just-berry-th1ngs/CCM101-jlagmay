# Mission Reflection

**1. Which cloud infrastructure component do you think is the most important? Why?**

I think networking is the most important component. Even if the compute resource is powerful and the storage holds perfectly accurate data, none of it matters if there's nothing to connect it to. In this lab, finding the server's hostname and IP address (Checkpoint 2) reminded me that a server is only reachable — and therefore only useful — because of its network identity. Without networking, cloud computing wouldn't even be possible, since the whole point is accessing a machine that isn't physically in front of you.

**2. How does Linux support cloud computing?**

Linux supports cloud computing by being open-source, lightweight, and stable, which keeps costs down for providers and lets them allocate resources to other things instead of licensing fees. This lab showed me that firsthand — KillerCoda let me simulate a real server environment without needing actual hardware or a paid operating system, using commands like lscpu, free -h, and df -h to inspect it just like a real cloud engineer would.

**3. Why is technical documentation important before deploying infrastructure?**

Documentation lets you know the capabilities of the hardware before you commit to deploying anything on it, without it, you risk putting a workload on a server that can't actually handle it. It also acts as a heads-up for other developers, so if they need to make changes or update settings later, they don't have to re-investigate the whole system from scratch to understand what they're working with.

**4. What new skills did you learn during this laboratory activity?**

I learned useful CLI commands for investigating my own hardware and system specs, like checking CPU, RAM, and disk info directly from the terminal instead of relying on a GUI. I'm also getting the hang of using CLI commands to manage Git — cloning, committing, and pushing changes — including resolving issues like the push rejection I ran into, which taught me how branches can diverge and how to reconcile them.

**5. How has your GitHub portfolio improved after completing this mission?**

My portfolio now looks like a well-thought-out body of work instead of just a single folder. It showcases what I've actually gone through — the investigation, the research, the diagram — along with a commit history that documents my progress and the improvements I still need to work on. Writing clearer commit messages this time also made the repo feel more like something a real engineer would maintain, not just a school submission.
