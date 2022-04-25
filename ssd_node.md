# SSD Note
[Applying UML And Patterns](https://personal.utdallas.edu/~chung/SP/applying-uml-and-patterns.pdf)

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
- [6. USE-CASE MODEL: WRITING REQUIREMENTS IN CONTEXT](#6-use-case-model-writing-requirements-in-context)
  - [6.1 Use Cases and Adding Value](#61-use-cases-and-adding-value)
  - [6.2 Use Cases and Functional Requirements](#62-use-cases-and-functional-requirements)
  - [6.3 Goals and Scope of a Use Case](#63-goals-and-scope-of-a-use-case)
    - [6.3.1 Scope of Use case](#631-scope-of-use-case)
    - [6.3.2 Goals of use case](#632-goals-of-use-case)
  - [6.4 Finding Primary Actors, Goals, and Use Cases](#64-finding-primary-actors-goals-and-use-cases)
  - [6.5 Actors](#65-actors)
  - [6.6 Requirements in Context and Low-Level Feature Lists](#66-requirements-in-context-and-low-level-feature-lists)
      - [6.6.1 High-Level System Feature Lists](#661-high-level-system-feature-lists)
  - [6.7 Use Cases Within the UP](#67-use-cases-within-the-up)
      - [6.7.1 Use Cases and Requirements Specification Across the Iterations](#671-use-cases-and-requirements-specification-across-the-iterations)
      - [6.7.2 Use Cases Within Inception](#672-use-cases-within-inception)
      - [6.7.3 Use Cases Within Elaboration](#673-use-cases-within-elaboration)
      - [6.7.4 Use Cases Within Construction](#674-use-cases-within-construction)
- [7. IDENTIFYING OTHER REQUIREMENTS](#7-identifying-other-requirements)
  - [7.1 Commentary: Supplementary Specification](#71-commentary-supplementary-specification)
  - [7.1.1 Quality Attributes](#711-quality-attributes)
  - [7.1.2 Domain (Business) Rules](#712-domain-business-rules)
  - [7.1.3 Information in Domains of Interest](#723-other-requirements-in-the-vision)
- [7.2 Commentary: Vision](#72-commentary-vision)
  - [7.2.1 System FeaturesóFunctional Requirements](#721-system-featuresófunctional-requirements)
  - [7.2.2 Other Requirements in the Vision](#722-other-requirements-in-the-vision)
  - [7.2.3 Vision, Features, or Use Cases Which First?](#723-vision-features-or-use-cases-which-first)
- [7.3 Commentary: Glossary (Data Dictionary)](#73-commentary-glossary-data-dictionary)
  - [7.3.1 Glossary as Data Dictionary](#731-glossary-as-data-dictionary)
- [8.FROM INCEPTION TO ELABORATION](#8from-inception-to-elaboration)
  - [8.1 On to Elaboration](#81-on-to-elaboration)
  - [8.2 Planning the Next Iteration](#82-planning-the-next-iteration)
  - [8.3 Iteration 1 Requirements and Emphasis: Fundamental OOA/D Skills](#83-iteration-1-requirements-and-emphasis-fundamental-ooad-skills)
## PART III ELABORATION ITERATION 1
- [9. Use-Case Model: Drawing System Sequence Diagrams](#9-use-case-model-drawing-system-sequence-diagrams)
  - [9.1 SSDs Within the UP](#91-ssds-within-the-up)



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
  - [6.1 Use Cases and Adding Value](#61-use-cases-and-adding-value)
  - [6.2 Use Cases and Functional Requirements](#62-use-cases-and-functional-requirements)
  - [6.3 Goals and Scope of a Use Case](#63-goals-and-scope-of-a-use-case)
    - [6.3.1 Scope of Use case](#631-scope-of-use-case)
    - [6.3.2 Goals of use case](#632-goals-of-use-case)
  - [6.4 Finding Primary Actors, Goals, and Use Cases](#64-finding-primary-actors-goals-and-use-cases)
  - [6.5 Actors](#65-actors)
  - [6.6 Requirements in Context and Low-Level Feature Lists](#66-requirements-in-context-and-low-level-feature-lists)
      - [6.6.1 High-Level System Feature Lists](#661-high-level-system-feature-lists)
  - [6.7 Use Cases Within the UP](#67-use-cases-within-the-up)
      - [6.7.1 Use Cases and Requirements Specification Across the Iterations](#671-use-cases-and-requirements-specification-across-the-iterations)
      - [6.7.2 Use Cases Within Inception](#672-use-cases-within-inception)
      - [6.7.3 Use Cases Within Elaboration](#673-use-cases-within-elaboration)
      - [6.7.4 Use Cases Within Construction](#674-use-cases-within-construction)

[Use-case template](https://docs.google.com/document/d/1Shx4J72A3HCzzHVCildE-UDN4dJOiZ5OKI3EdoAA42w/edit) (KU-mail)  
Example: [use-case model](https://docs.google.com/document/d/1aC0IudRNPjrG9g-y2AHBf5j9GEzy-6HkX6juhp0B0W8/edit) (KU-mail)   
    
    A stories of using a system to meet goals.
    A collection of related success and failure scenarios that describe actors using a system to support a goal.

![image8](/image/8.png)

## 6.1 Use Cases and Adding Value
| Use Cases component | Definition |
| ------------| -----------|
| [Goals](#goals-of-use-case) | The thing that user want to achive by using application. |
| [Actors](#65-actors)  |  It is something with behavior, such as a person (identified by role), computer system |
| Scenario | A specific sequence of actions and interactions between actors and the system under discussion |

**Note** Take a look on [Use-case template](https://docs.google.com/document/d/1Shx4J72A3HCzzHVCildE-UDN4dJOiZ5OKI3EdoAA42w/edit) to see other component.

A key attitude in use case work is to focus on the question "How can using the system provide observable value to the user, or fulfill their goals?", rather than merely thinking of system requirements in terms of a "laundry list" of features or functions.

## 6.2 Use Cases and Functional Requirements
Use cases are requirements that indicate what the system will do. Use cases define a promise or contract of how a system will behave.

    Use cases are requirements

**Note** Use cases are text documents, not diagrams</br>
</br>

## 6.3 Goals and Scope of a Use Case

### 6.3.1 Scope of Use case
![image7](/image/7.png)

EBP : A task performed by one person in one place at one time, in response to a business event, which adds measurable business
value and leaves the data in a consistent state.  
**Note** Use case is not fail as an EBP if two people are required, or if a person has to walk around.</br>
</br>

### 6.3.2 Goals of use case
Actors have goals (or **needs**) and use applications to help satisfy them. In fact, the name of a use case for a user goal should reflect its name</br>
</br>

## 6.4 Finding Primary Actors, Goals, and Use Cases

| Finding Step | 
| ------------| 
| Step 1: Choosing the System Boundary | 
| Steps 2 and 3: Finding Primary [Actors](#65-actors) and Goals  | 
| Step 4: Define Use Cases |    

**Note** An actor depent on boundary.</br>   
![image9](/image/9.png)

## 6.5 Actors
An actor is anything with behavior, including the system. Actors are not only roles played by people, but organizations, software, and machines.

| Actor |           | Why identify?
| ------------| ------------| ------------|
| Primary actor | has user goals fulfilled through using services of the SuD. | To find user goals, which drive the use cases.|
| Supporting actor | provides a service (for example, information) to the SuD. |To clarify external interfaces and protocols.|
| Offstage actor | has an interest in the behavior of the use case, but is not primary or supporting.  | To ensure that all necessary interests are identified and satisfied. |

**Note** SuD : system under discussion.</br>
</br>

## 6.6 Requirements in Context and Low-Level Feature Lists
Some non-functional requirements, domain rules and context, and other hard-to-place elements are better captured in the Supplementary Specification. One idea behind use cases is to replace detailed, low-level feature lists. These lists tended to look as follows, usually grouped into functional areas:  

![image10](/image/10.png)</br>
</br>

### 6.6.1 High-Level System Feature Lists
The list provides a very succinct summary of system functionality, independent of the use case view.</br>
</br>
![image11](/image/11.png)</br>
</br>

## 6.7 Use Cases Within the UP
Use cases are vital and central to the UP, which encourages use-case driven development.  
This mean: 
1. Requirements are primarily recorded in use cases
2. Use cases are an important part of iterative planning.
3. Use-case realizations drive the design. That is, the team designs collabo rating objects and subsystems in order to perform or realize the use cases.
4. Use cases often influence the organization of user manuals

**Note** Business use cases are less commonly written.

### 6.7.1 Use Cases and Requirements Specification Across the Iterations
</br>

![image12](/image/12.png)</br>
</br>

### 6.7.2 Use Cases Within Inception
Not all use cases are written in their fully dressed format during the inception phase. In order to decide if the project is worth significant investigation (that is, the elaboration phase). The inception work is not meant to do that investigation, but to obtain low-fidelity (and admittedly error-prone) insights regarding scope, risk, effort, technical feasibility, and business case, in order to decide to move forward, where to start if they do, or if to stop.</br>
</br>

### 6.7.3 Use Cases Within Elaboration
This is a phase of multiple timeboxed iterations (for example, four iterations) in which risky, high-value, or architecturally significant parts of the system are incrementally built, and the "majority" of requirements identified and clarified. </br>
</br>

### 6.7.4 Use Cases Within Construction
The construction step is composed of timeboxed iterations that focus on completing the system, once the risky and
core unstable issues have settled down in elaboration. There will still be some **minor** use case writing</br>
</br>

# 7. IDENTIFYING OTHER REQUIREMENTS
- [7.1 Commentary: Supplementary Specification](#71-commentary-supplementary-specification)
  - [7.1.1 Quality Attributes](#711-quality-attributes)
  - [7.1.2 Domain (Business) Rules](#712-domain-business-rules)
  - [7.1.3 Information in Domains of Interest](#723-other-requirements-in-the-vision)
- [7.2 Commentary: Vision](#72-commentary-vision)
  - [7.2.1 System FeaturesóFunctional Requirements](#721-system-featuresófunctional-requirements)
  - [7.2.2 Other Requirements in the Vision](#722-other-requirements-in-the-vision)
  - [7.2.3 Vision, Features, or Use Cases Which First?](#723-vision-features-or-use-cases-which-first)
- [7.3 Commentary: Glossary (Data Dictionary)](#73-commentary-glossary-data-dictionary)
  - [7.3.1 Glossary as Data Dictionary](#731-glossary-as-data-dictionary)

## 7.1 Commentary: Supplementary Specification
**The Supplementary Specification** captures other requirements, information, and constraints not easily captured in the use cases or Glossary, including system-wide "URPS+" quality attributes or requirements. Supplementary Specification.. Elements of the Supplementary Specification could include:       
1. FURPS+
2. reports 
3. hardware and software constraints (operating and networking systems, ...) 
4. development constraints (for example, process or development tools)
5. other design and implementation constraints 
6. internationalization concerns (units, languages, ...) 
7. documentation (user, installation, administration) and help
8. licensing and other legal concerns 
9. packaging
10. standards (technical, safety, quality)
11. physical environment concerns (for example, heat or vibration)
12. operational concerns (for example, how do errors get handled, or how often to do backups?) 
13. domain or business rules
14. information in domains of interest (for example, what is the entire cycle of credit payment handling?) 

**Constraints** are not behaviors, but some other kind of restriction on the design or project. They are also requirements, but are commonly called "constraints" to emphasize their restrictive influence.</br>
</br>

![image13](/image/13.png)</br>
</br>

### 7.1.1 Quality Attributes 
Some requirements are called **quality attributes** of a system. These refer to the qualities of the system. They are of two types:
1. Observable at execution (functionality, usability, reliability, performance, ...)
2. Not observable at execution (supportability, testability, ...) 

### 7.1.2 Domain (Business) Rules
It is often useful to identify and record those domain rules that influence the requirements, usually realized in the use cases, because they can clarify incomplete or ambiguous use case content.</br>
</br>

![image14](/image/14.png)</br>
</br>

### 7.1.3 Information in Domains of Interest
An explanation of domains related to the new software system to provide context and deeper insight for the development team. It may contain pointers to important literature or experts, formulas, laws, or other references.

## 7.2 Commentary: Vision
| Are We Solving the Same Problem? The Right Problem?          | |
| ------------| ------------| 
| The Problem Statement| In the inception phase, collaborate to define a terse problem statement| 
| The Key High-Level Goals and Problems of the Stakeholders | <center>![image15](/image/15.png)</br> </br>This table summarizes the goals and problems at a higher level than task level use cases|
|What Are the Root Problems and Goals?| Sometimes stakeholder jump to solutions that are not the most appropriate or do not address the root underlying major problems. |
| Group Idea Facilitation Methods | Techniques to discover root problems and goals, and support idea generation and prioritization |

### 7.2.1 System Features Functional Requirements

Use cases are not necessarily Why?
1. Stakeholders often want a short summary that identifies the most noteworthy functions.
2. The list may still be too long. Also, the names can hide interesting functionality stakeholders really want to know about
3. Some noteworthy functionality is naturally expressed as short statements that do not conveniently map to use case names or Elementary Business Process-level goals

Therefore, an alternative, a complementary way to express system functions is with features, or more specifically in this context, system features, which are high-level, terse statements summarizing system functions.

![image16](/image/16.png)</br>

**Vision** may be used as a formal or informal contract between development and business. System features are a mechanism to summarize in this contract what the system will do. This is complementary to the use cases, as the features are terse.

### 7.2.2 Other Requirements in the Vision
Vision can summarize other requirements (for example, reliability and usability) that are detailed in the Special Requirements sections of use cases, and in the Supplementary Specification

![image17](/image/17.png)

### 7.2.3 Vision, Features, or Use Cases Which First?
1. Write a brief first draft of the Vision. 
2. Identify user goals and the supporting use cases. 
3. Write some use cases and start the Supplementary Specification.
4. Refine the Vision, summarizing information from these. 

## 7.3 Commentary: Glossary (Data Dictionary)
**Glossary** is a list of noteworthy, unclear, ambiguous, terms and their definitions. It is surprisingly common that a term, often technical or particular to the domain

![image18](/image/18.png)

### 7.3.1 Glossary as Data Dictionary
Glossary a data dictionary, a document that records data about the dataóthat is, metadata.
Term attributes could include:
1. aliases
2. description 
3. format (type, length, unit)
4. relationships to other elements
5. range of values
6. validation rules

**Units**  must be considered, especially in this age of internationalized software applications.

The Glossary is not only for atomic terms It can and should include composite elements and nicknames used to describe a collection of
data transmitted between actors in the use cases

![image19](/image/19.png)

Instead of being plain static documents, they may be hyperlinked, or recorded in tools other than a word processor or spreadsheet.

# 8.FROM INCEPTION TO ELABORATION
- [8.1 On to Elaboration](#81-on-to-elaboration)
- [8.2 Planning the Next Iteration](#82-planning-the-next-iteration)
- [8.3 Iteration 1 Requirements and Emphasis: Fundamental OOA/D Skills](#83-iteration-1-requirements-and-emphasis-fundamental-ooad-skills)

## 8.1 On to Elaboration
Elaboration is the initial series of iterations during which the team does serious investigation, implements (programs and tests) the core architecture, clarifies most requirements, and tackles the high-risk issues.

![image20](/image/20.png)

Some key ideas and best practices that will manifest in elaboration include:
1. do short timeboxed risk-driven iterations
2. start programming early 
3. adaptively design, implement, and test the core and risky parts of the architecture
4. test early, often, realistically 
5. adapt based on feedback from tests, users, developers 
6. write most of the use cases and other requirements in detail, through a series of workshops, once per elaboration iteration   </br>

Elaboration phase testing is important, to obtain feedback, adapt, and prove that the core is robust.

## 8.2 Planning the Next Iteration
Planning and project management are important but large topics. Some key ideas are briefly presented.Organize requirements and iterations by risk, coverage, and criticality.
1. **Risk** includes both technical complexity and other factors, such as uncer tainty of effort or usability.
2. **Coverage** implies that all major parts of the system are at least touched on in early iterations perhaps a "wide and shallow" implementation across many components.
3. **Criticality** refers to functions of high business value.

In terms of UP artifacts:
1. The chosen requirements for the next iteration are briefly listed in an **Iteration Plan**. This is not a plan of all the iterations, only a plan of the next. 
2. A task or requirement for the iteration may be written in greater detail in a separate **Change Request**, and given to the responsible party. 
3. The overall requirements ranking is recorded in the **Software Development Plan**.

## 8.3 Iteration 1 Requirements and Emphasis: Fundamental OOA/D Skills
Iteration 1 of the elaboration phase emphasizes a range of fundamental and common OOA/D skills used in building object systems, such as assigning responsibilities to objects.

Iteration 1 Requirements
1. Implement a basic, key scenario
2. Implement a Start Up use case as necessary to support the initialization needs of the iteration. 
3. Nothing fancy or complex is handled, just a simple happy path scenario, and the design and implementation to support it
4. There is no collaboration with external services.
5. No complex pricing rules are applied. </br>
</br>

       Incremental Development for the Same Use Case Across Iterations

# 9. Use-Case Model: Drawing System Sequence Diagrams
- [9.1 SSDs Within the UP](#91-ssds-within-the-up)

**Sequence Diagrams**: describe the system behavior, what a system does, without explaining how it does it, a picture that shows, for a particular scenario of a use case, the events that external actors generate, their order, and inter-system events to illustrate collaborations between systems.   
![image21](/image/21.png)

SSDs and Use Cases: An SSD shows system events for a scenario of a use case, therefore it is generated from inspection of a use case.

![image22](/image/22.png)</br>

**Note**: 
1. The boundary is very important(Take a look at [Chapter6](#63-goals-and-scope-of-a-use-case))
2. Naming should be expressed at the level of intent rather than in terms of the physical input medium or interface widget level.

## 9.1 SSDs Within the UP
SSDs are part of the Use-Case Model a visualization of the interactions implied in the use cases.   
**Inception**: SSDs are not usually motivated in inception.   
**Elaboration**: Most SSDs are created during elaboration, when it is useful to identify the details of the system events to clarify what major operations the system must be designed to handle, 

![imgae23](/image/23.png)

# 10. IN MODEL VISUALIZING CONCEPTS

## 10.1 Domain Models
**Domain model** is a visual representation of conceptual classes or real-world objects in a domain of interest also been called **conceptual models**

**Class Diagrams** may shown:
1. domain objects or conceptual classes
2. associations between conceptual classes 
3. attributes of conceptual classes

![image24](/image/24.png)

The domain model may be considered a visual dictionary of the noteworthy abstractions, domain vocabulary, and information content of the domain. It is a visualization of things in the real world domain of interest, not of software components.

Element are not suitable in a domain model:
1. Software artifacts, such as a window or a database.
2. Responsibilities or methods.

|This| Not this|
|----|---------|
|![image25](/image/25.png)| ![image26](/image/26.png)|

**Conceptual Classes** is an idea, thing, or object and may be considered in terms of its symbol, intension, and extension.

|Conceptual Classes| |
|------------------|-|
|Symbol|words or images representing a conceptual class.|
|Intension|the definition of a conceptual class.|
|Extension|the set of examples to which the conceptual class applies.|

![image27](/image/27.png)

Decomposition divide-and-conquer is a common strategy to deal with this complexity by division of the problem space into comprehensible units.

## 10.2 Conceptual Class Identification
three techniques are presented in the following sections:
1. Use a conceptual class category list. 
2. Identify noun phrases
3. use an existing model   

A weakness of this approach is the imprecision of natural language; different noun phrases may represent the same conceptual class or attribute, among other ambiguities.

**Note**: The most common mistake when creating a domain model is to represent something as an attribute when it should have been a concept.

## 10.3 Lowering the Representational Gap
Choosing names that reflect the domain vocabulary (Sale) enhances quick comprehension and provides a clue as to what to expect from the chunk of code

**representational gap** or semantic gap—the gap between our mental model of the domain and its representation in software.