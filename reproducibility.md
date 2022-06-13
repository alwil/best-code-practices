---
marp: true
title: Reproducibility
paginate: false
theme: custom
backgroundColor: #fff

---
# Writing reproducible code


---
# How do you currently develop your code?

- Tools
- Collaborators
- Storage
- Sharing

Are you happy with the way you currently work?

---
# The FAIR principles

Original paper demands that all scholarly digital research objects should be findable,
accessible, interoperable, and reusable

Increasingly recognized as essential for the transition towards Open Science

![bg right:40% width:500](./img/FAIR_paper.png)


---
# Would this be enough?
- Access to the code
- Access to the data
- (And let's assume we can replicate the environment)

How confident do you feel?

---
# Is this enough?
- Access to the code
- Access to the data
- (And let's assume we can replicate the environment)

How confident do you feel?

**We need to do more to inspire trust**
- The code is correct (and I have made it easy for you/someone to check)
- My workflow is robust
- My workflow _itself_ is accessible, and I will be guiding you through it.

---
# What is research reproducibility?

![bg right:60% height:550](./img/reproducible-definition-grid.jpg)

>Science that cannot be verified, is not science. How about code?

---
# Advantages of reproducible code

1. Track a complete history of your research
2. Facilitate collaboration and review process
3. Publish validated research and avoid misinformation
4. Write your papers, thesis and reports efficiently
5. Get credits for your work fairly
6. Ensure continuity of your work

---
![width:1000](./img/barriers-reproducibility.png)

---
## Be aware of the human side
- No credit
- Lacking programming skills
- Sharing anxiety - Am I good enough? --> imposter syndrome

![bg right:50% height:400](./img/make-ok-to-be-human.jpg)

---
# Reproducibility crisis

Is current science reproducible?

---
# Lacking method decription

Black box offered as scientific method:
- "Method is adapted from..." and additional steps only superficially described
- Method named, but details missing
- Complex models with no available code or even executable tools

![height:300](./img/Blackbox3D-withGraphs.png)

# Method and data
>When results are produced by complex computational processes using large volumes of data, the methods section of a traditional scientific paper is insufficient to convey the necessary information for others to reproduce the results.

**Recommendations**
- Provide input, intermediate, and output data
- Provide detailed methods, ideally in executable format
- Provide information about the computational environment

---
# What is a computational environment
> Information about the computational environment where the study was originally executed, such as operating system, hardware architecture, and library dependencies.

Do you think this is sufficient?

---
## You should also consider...

- versions of dependencies (and their interoperability)
- configuration files and databases
- required (commercial) licenses, e.g. MATLAB
- tool for managing OS dependency (containers)
- for interactive systems, all user input provided by the user
- locales (language conventions)

![bg right:40% width:500](./img/python_environment.png)

---
# Exercize

Inspect your project and identify issues with reproducibility

---
![width:1200](./img/Glerean_continuum_best_practices1800.png)

---
# How can you measure FAIR

- The Netherlands eScience Center's "Five Recommendations for FAIR Software" (https://fair-software.nl) and 


---
# Steps towards reproducibility
1. Make sure you can find it (in space)
1. Make sure you can find it (in time)
1. Make sure you can recreate the environment where it lived at a specific time
1. Make sure you can execute the same sequence of operations
1. Make sure your environment and sequence of operations is robust and no human is needed to replicate what was done

---
# Steps towards replicable & robust code
1. Remove hardcoded bits and make the code modular
2. Test that the modules you made can take different types of input data or parameters
3. Turn the modules into a package/toolbox

---
# Steps towards generalisable code
1. License your code and get citations
2. Make sure your code is readable by humans
3. Make sure comments are present
4. Write useful documentation

---
# Metrics for  FAIR for Research Software


