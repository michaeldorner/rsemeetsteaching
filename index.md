# How to tap the minds of the brightest students for RSE?

Software underpins almost all research and is, in one way or another, at the core of scientific discovery today. We rely on high-quality and reliable software for high-quality and reliable results. Therefore, the engineering of such research software cannot be an afterthought. Research Software Engineering (RSE) bridges this gap between the complex demands of scientific research and the need for reliable, maintainable, and reliable software solutions for researchers. That makes us researchers and software engineers. 
But as researchers, we are also teachers. So the question comes naturally: How can we tap the minds of our brightest students for research software engineering?

In this experience report, we reflect on our approach to integrating research software engineering as part of the regular curriculum for software engineering students at Blekinge Institute of Technology, Sweden. 


# Experimental design

## Teaching

The course introduces hands-on testing and quality assurance techniques for software systems for students from the SE and AI B.Sc. programmes. 

The instance of the course we experiment with took place in Spring 2023. 40 students enrolled the course as part of their curriculum. 

## Research and research software

As research software, we selected a real-world simulation for information diffusion in code reviews at Microsoft, Spotify, and Trivago modelled as networks. As we implemented Dijkstra’s algorithm for time-varying hypergraphs in Python and the code review systems are partially huge (e.g., Microsoft's code review consists of over 30.000 developers), the simulation is computational expensive: On conventional hardware, it takes several days to simulate all information spreads and process the results. 

Initially, the code had only a bare minumum testing suite. 

## Integration

We integrated the research software as practical group projects. Each group consisted of 4 or 5 students. Each project group must implement a minimum test suite for a CI-pipeline and choose a project focus. The  (e.g., performance testing or algorithmic verification)

# Evaluation and Reflection

## The Good

As a result of the integration, we observed three main benefits for our research software at hand. 

Our research software grew a comprehensive test suite. The test suite containes now unit and integration tests to catch regression bugs. Two projects went even beyond classical testing and developed fuzzing tests to catch memory-corruption and safety bugs. The test suite now enables to ensure that software artifacts meet their requirements. <!---andi das geht bestimmt besser oder?-->

To ease the barriers for students at the project start, we improved the documentation in size and quality. The improved documentation is beneficial not only for students, but also for other researchers reproducing or replicating our simulation. <!---andi schreibt was über warum docu gut ist--->

We did not provide a unified hardware setup but relied on the students' computers. To cover the large diveristies in hardware, operating systems, and software environments, we removed all OS and hardware requirements and minimized code dependencies. <!---andi schreibt was über warum weniger dependencies besser ist-->

## The Bad

However, there is no such thing as a free lunch. We had substantial efforts—upfront and continous—for improving documentation context and minimizing dependencies and requirements. 

## The Ugly

The biggest drawback we found was the uncertainty about intellectual property of student contributions. That hindered us to integrate the code from students in our software.

# Conclusion


