# SSD Note
[Applying Uml And Patterns](https://personal.utdallas.edu/~chung/SP/applying-uml-and-patterns.pdf)

## PART I INTRODUCTION
- [SSD Note](#ssd-note)
- [1. Object-Oriented Analysis and Design](#1-object-oriented-analysis-and-design)
  - [1.1 Assigning Responsibilities](#11-assigning-responsibilities)
  - [1.2 What Is Analysis and Design?](#12-what-is-analysis-and-design)
  - [1.3 What Is Object-Oriented Analysis and Design?](#13-what-is-object-oriented-analysis-and-design)
- [2. ITERATIVE DEVELOPMENT AND THE **UNIFIED PROCESS**](#2-iterative-development-and-the-unified-process)
  - [2.1 Iterative development](#21-iterative-development)
  - [2.2 The UP Phases and Schedule Oriented Terms](#22-the-up-phases-and-schedule-oriented-terms)
  - [2.3 The UP Disciplines](#23-the-up-disciplines)
- [3. CASE STUDY: THE NEXTGEN POS SYSTEM](#3-case-study-the-nextgen-pos-system)
  - [3.1 Architectural Layers and Case Study Emphasis](#31-architectural-layers-and-case-study-emphasis)
## PART II INCEPTION
- [4. Inception](#4-inception)
  - [4.1 Inception: An Analogy](#41-inception-an-analogy)
  - [4.2 Inception May Be Very Brief](#42-inception-may-be-very-brief)
  - [4.3 What Artifacts May Start in Inception?](#43-what-artifacts-may-start-in-inception)
- [5. UNDERSTANDING REQUIREMENTS](#5-understanding-requirements)
  - [5.1 Types of Requirement](#51-types-of-requirement)



# 1. Object-Oriented Analysis and Design
  - [1.1 Assigning Responsibilities](#11-assigning-responsibilities)
  - [1.2 What Is Analysis and Design?](#12-what-is-analysis-and-design)
  - [1.3 What Is Object-Oriented Analysis and Design?](#13-what-is-object-oriented-analysis-and-design)
## 1.1 Assigning Responsibilities

    A critical, fundamental ability in OOA/D is to skillfully assign responsibilities to software components.

Because it is one activity that must be performed—either while drawing a
UML diagram or programming—and it strongly influences the robustness,
maintainability, and reusability of software components.<br />
<br />

## 1.2 What Is Analysis and Design?
| What Is Analysis and Design            | Definition               |
| ----------------- | -------------------- |
| Analysis           | an **invertigation of problem and requirement**, rather than a solution               |
| Design            | a **conceptual solution which is fullfill the requirement**, rather than implement     |   

As with analysis, the term is best qualified, as in object design or database design.  
```"phase do the right thing (analysis), and do the thing right (design)."```<br />
<br />

## 1.3 What Is Object-Oriented Analysis and Design?
| What Is Analysis and Design            | Definition               |
| ----------------- | -------------------- |
| object-oriented analysis          | finding and describing the objects or concepts in the problem domain. |
| object-oriented design            |defining software objects and how they collaborate to fulfill the requirements. |   

![image4](/image/4.png)<br />
<br />   

``` Define use case ``` -> ``` Define domain model ``` -> ``` Define interact diagrams ``` ->  ``` Define dising class diagram ```


| Define            | Description                                                                                |
| ----------------- | ------------------------------------------------------------------------------------------ |
| Use case          | It is a simply written stories.                                                            | 
| Domain model      | Expressed a set of diagrams that show domain concepts or objects.                          |
| Interact diagrams | It shows the flow of messages between software objects, and thus the invocation of methods.|
| Class diagrams    | illustrates the attributes and methods of the classes.                                     |
<br />

# 2. ITERATIVE DEVELOPMENT AND THE **UNIFIED PROCESS**
  - [2.1 Iterative development](#21-iterative-development)
  - [2.2 The UP Phases and Schedule Oriented Terms](#22-the-up-phases-and-schedule-oriented-terms)
  - [2.3 The UP Disciplines](#23-the-up-disciplines)  
      - [2.3.1 Disciplines and Phases](#231-disciplines-and-phases)

## 2.1 Iterative development
    It is organized into a series of short, fixed-length mini-projects called iterations; the outcome of each is a tested integrated, and executable system. Each iteration includes its own requirements analysis, design, implementation, and testing activities.
<br />

## 2.2 The UP Phases and Schedule Oriented Terms


| UP Process  | Definition |
| ------------| -----------|
| [Inception](#4-inception)   | approximate vision, business case, scope, vague estimates.| 
| Elaboration | refined vision, iterative implementation of the core architecture, resolution of high risks, identification of most requirements and scope,more realistic estimates.|
| Construction | iterative implementation of the remaining lower risk and easier elements, and preparation for deployment.|
| Transition    | beta tests, deployment.|

**Note** : This is not the old "waterfall" or sequential lifecycle of first defining all the requirements, and then doing all or most of the design.<br />
<br />

## 2.3 The UP Disciplines
The UP describes work activities such as writing a use case, within disciplines (originally called workflows). The discipline is  a set of activities (and related artifacts) in one subject area, such as the activities within requirements analysis  
![image2](/image/2.png)</br>
</br>

### 2.3.1 Disciplines and Phases
The relative effort across these disciplines changes over time.
Early iterations naturally tend to apply greater relative emphasis to requirements and design, and later ones less so, as the requirements and core design
stabilize through a process of feedback and adaptation.
![image3](/image/3.png)</br>
</br>

# 3. CASE STUDY: THE NEXTGEN POS SYSTEM
 - [3.1 Architectural Layers and Case Study Emphasis](#31-architectural-layers-and-case-study-emphasis)
## 3.1 Architectural Layers and Case Study Emphasis
A typical object-oriented information system is designed in terms of several rchitectural layers or subsystems
| Architectural Layers  | Definition |
| ------------| -----------|
| User Interface | graphical interface; windows |
| Application Logic and Domain Objects | software objects representing domain concepts that fulfill application requirements. |
| Technical Services (Framework) | provide supporting technical services, such as interfacing with a database or error logging. These services are usually application-independent and reusable across several systems. |

![image5](/image/5.png)</br>
</br>

# 4. Inception
  - [4.1 Inception: An Analogy](#41-inception-an-analogy)
  - [4.2 Inception May Be Very Brief](#42-inception-may-be-very-brief)
  - [4.3 What Artifacts May Start in Inception?](#43-what-artifacts-may-start-in-inception)  

Some requirements exploration **but not define all the requirements**. The inception phase should be relatively short for most projects, such as
one or a few weeks long.

**Note**: It is to decide if the project is worth a serious investigation (during elaboration), not to do that investigation.
![image6](/image/6.png) </br>
</br>

## 4.1 Inception: An Analogy
It is premature there is insufficient information. Inception phase is akin to a feasibility study to decide if it is even worth investing in exploratory drilling. Only after exploration (elaboration) do we have the data and insight to make somewhat believable estimates and plans.  

```estimates are not to be considered reliable in the inception phase.```

In UP terms, the realistic exploration step is the **elaboration phase**<br />
<br />

## 4.2 Inception May Be Very Brief
The intent of inception is to establish some initial common vision for the objectives of the project, determine if it is feasible, and decide if it is worth some serious investigation in elaboration.<br />
<br />

## 4.3 What Artifacts May Start in Inception?
| Artifact  | Comment |
| ------------| -----------|
| Vision and Business Case  | Describes the high-level goals and constraints, the business case, and provides an executive summary.|
| [**Use-Case Model**](#6-use-case-model-writing-requirements-in-context)  | Describes the functional requirements, and related non-functional requirements. |
| Supplementary Specification  | Describes other requirements.  |
| **Glossary**   | Key domain terminology.  |
| Risk List & Risk Management Plan  | Describes the business, technical, resource, schedule risks, and ideas for their mitigation or response.  |
| Prototypes and proof-of-concepts   | To clarify the vision, and validate technical ideas.  |
| **Iteration Plan**   | Describes what to do in the first elaboration iteration.  |
| Phase Plan & Software Development Plan  | Low-precision guess for elaboration phase duration and effort. Tools, people, education, and other resources.  |
| Development Case   | A description of the customized UP steps and artifacts for this project. In the UP, one always customizes it for the project.  |</br>
</br>

# 5. UNDERSTANDING REQUIREMENTS
  - [5.1 Types of Requirement](#51-types-of-requirement)  

**Requirements** are capabilities and conditions to which the system—and more broadly, the project—must conform.</br>
</br>

## 5.1 Types of Requirement
| FURPS+ model  | Definition |
| ------------| -----------|
| [F] unctional  | features, capabilities, security. |
| [U] sability  | human factors, help, documentation. |
| [R] eliability  | frequency of failure, recoverability, predictability. |
| [P] erformance  | response times, throughput, accuracy, availability, resource usage.|
| [S] upportability  | adaptability, maintainability, internationalization, configurability.  |
| [+] Implementation  | resource limitations, languages and tools, hardware, ... |
| [+] Interface  | constraints imposed by interfacing with external systems. |
| [+] Operations  | system management in its operational setting. |
| [+] Packaging   | - |
| [+] Legal  | licensing and so forth. |

In common usage, requirements are categorized as functional (behavioral) or non-functional (everything else)   
**Note** Functional requirements are explored and recorded in the [**Use-Case Model**](#6-use-case-model-writing-requirements-in-context)</br>
</br>

# 6. USE-CASE MODEL: WRITING REQUIREMENTS IN CONTEXT
