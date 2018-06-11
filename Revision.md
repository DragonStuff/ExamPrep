# Topics

- UML modelling 
	- The “4+1” view 
	- Logical view 
		- Class and object diagrams 
		- Packages 
		- State diagrams 
	- Process view 
		- Sequence diagrams 
		- Communication diagrams 
		- Activity diagram 
		- Interaction Overview Diagrams 
	- Deployment view 
		- Deployment diagrams 
	- Implementation view 
		- Composite diagrams 
		- Component diagrams 
	- UML diagrams and RUP
- Agile methods
	- Agile principles
	- Scrum
	- Extreme Programming
	- Dynamic Systems Development Method
- Rational Unified Process (RUP)
- Software testing and Test-Driven Development
	- Verification and validation
	- Static verification (software inspection)
	- Dynamic verification (software testing)
	- Test-driven development
- DevOps
- Capability Maturity Model Integration (CMMI) model

# Questions

- Theoretical questions
	- Describe and explain a certain concept
- E.g. Explain the waterfall process model.
- E.g. What activities take place during the construction phase of a RUP project and what are the principal artefacts produced in this phase?
- E.g. Briefly describe the main meetings held if one follows the Scrum methodology.
- Practical questions
	- You are given a description of a system and are asked to develop a UML model (e.g. use case diagram, class diagram, sequence diagram, state diagram, activity diagram, etc.)
	- Similar to the exercises we went through in the labs. 

# Lecture 2

Software engineering has two main components.
- PRODUCT - The actual software product or system that is built and put into operation.
- PROCESS - A framework for the tasks that are required to build high-quality software.

Engineering knowledge encompasses scheduling, costing, estimating, building, testing, communicating and organising.

Software does not wear out, no physical laws, specifications constantly changes. Software does not need to have its copies mass produced, it is copied near-instantly.

- Software Engineering Development Activities
	- Planning 15% EFFORT (PERSON MONTHS)
		+ Identify business value
			* Develop a System Request to initiate the project (approved by management)
				- This identifies the business value of the new system
				- Contains business need
				- Functionality at a high level
				- Expected value such as an increase in sales, stability
				- Expected issues or constraints
		+ Analyse feasibility
			* Feasibility study by business analyst - Consequences
				- Technical - Can it be built? Are we familiar with the technology or type of system? Size of system?
				- Economic - Cost v Benefit analysis (development and operational costs, tangible/intangible costs or benefits) & ROI
				- Organisational - Will the system be accepted by the users and integrated into the organization? Who is affected?
		+ Develop work plan
			* Work Breakdown Structure
				- Identify tasks/subtasks
				- Estimate time taken
				- Deliverables per task
				- Assign tasks
		+ Staff the project
		+ Estimate
			* Constructive Cost Model - effort = c x size^k
				- Organic - Small team, small system, in-house, flexible
				- Embedded - Tight constraints, expensive
				- Semi-detached - Mixture of the two
		+ Identify risk
			* Find risks
			* Classify risks
			* Rank risks
			* Prevention and Response planning
				- AVOID
				- TRANSFER
				- ASSUME
	- Requirements 20% EFFORT (PERSON MONTHS) - WHAT TO BUILD
		+ Requirements elicitation
			* Who are stakeholders, what do they expect
			* Perform interviews, quiz, meetings
		+ Requirements specification
			* Define requirements in detail
			* Define use cases
			* Software Requirements Specification
	- Design 35% EFFORT (PERSON MONTHS) - HOW TO BUILD
		+ Architectual design
			* Major structure of the software (like blueprint)
		+ Subsystem design
			* Interfaces and protocols, structure (packages/components)
		+ Detailed design
			* Describe classes, methods, attributes/data-types
		+ Persistent data design
			* Describe database, tables, primary and foreign keys
		+ GUI design
			* UI DESIGN, how it will look, tools, structure, design/style guidelines
	- Implementation 30% EFFORT (PERSON MONTHS)
		+ Construction
			* Write code!
		+ Installation/Deployment
			* Deploy it into the environment
	- Verification and validation
		+ Verification
			* Working state
			* Use case testing
			* Conformance to specification
			* System testing involves executing the system with test cases that are derived from the specification of the real data to be processed by the system.
		+ Validation
			* Meeting requirements of system customer
	- Maintenance and evolution
		+ Adaptive maintenance
			* Changing according to environment
		+ Corrective maintenance
			* Fixing errors/bugs
		+ Perfective maintenance
			* Changing to new needs

		+ If the users find they can get work done with the new system, then they will soon identify additional tasks for it to do and require changed forms for interaction with the system.

---

# Lecture 3

- Many different processes but they all involve:
	- Requirements specification - defining what the system should do;
	- Design & Implementation - defining the organization of the system and implementing the system
	- Verification & Validation (V & V) - checking that it conforms to the specification and does what the customer wants
	- Maintenance and Evolution - changing the system in response to changing customer needs.
	- A structured set of activities required to develop a software system
	- A software process model is an abstract representation of a process. It presents a description of a process from some particular perspective

- Software process models
	- Waterfall model
		+ Phase by phase, must be complete and correct before the next phase. Top to bottom, standard manufacturing methodology.
		+ Need to fully understand problem and have a completely correct design before implementation can begin.
		+ Needs well understood requirements.
		+ Hardest and most expensive to use.
	- Prototyping model
		+ Parts
			* Requirement gathering
			* Quick design
			* Build prototype - SHOULD BE DISPOSIBLE
			* Customer evaluation
			* Refine, iterate to quick design if not approved
			* Make the product
		+ Benefits
			* Users involved
			* Reduced time/costs
		+ Limitations
			* Users may think prototype is completed system
			* Developer may alter requirements to prototype
			* Potential for excessive prototype development time
			* Expense of implementing prototyping (constant dev)
	- Iterative/incremental model
		+ Parts
			* Develop through repeated cycles in small portions
			* Prioritise user requirements, increments start with highest
			* Each iteration introduces features
		+ Benefits
			* LESS RISK
			* Feedback in early stages used for later stages
			* Reduced cost of requirement changes
			* Rapid delivery and deployment of useful software
			* Early increments similar to prototypes
			* Highest priority requirements have extensive testing
		+ Limitations
			* Higher costs due to repeats of same costs
			* Degraded core of software
			* Further changes are expensive
	- Spiral model
		+ Mixture of prototyping and iterative models
		+ Spiral rather than a sequence
		+ Used in large projects such as game development 
	- Rational Unified Process
		+ 
	- Agile development
		+ Focus on code, iterative approach
		+ Deliver quickly and evolve quickly

---

# Lecture 4

UML is a modelling language

- Two important components of a software development methodology:
	+ Process (discussed in the previous lecture)
	+ Modelling language
- What is a model?
	+ A model describes a system using a well defined (modelling) language, which has clear syntax and semantics suitable for both human and computer interpretation.

- Structural model
	+ “Class” diagrams.
		* the structure and substructure of the system using objects, attributes, operations, and relationships.
- Functional model
	+ “Use case” diagrams.
		* The functionality of the system from the user's point of view
- Behavioural model
	+ Sequence diagrams, activity diagrams and state machine diagrams
		* The internal behaviour of the system

- Use Case Diagrams
	+ Information
		* Use cases are from the USERS's POINT OF VIEW
		* Interaction between system and user/other system
			- Example: A borrower borrows a book (Library System)
		* Functional description of the system is the collection of all use cases
		* Model functional requirements as Actors interacting with Use Cases
	+ Structure
		* Join - Solid line with NO ARROW between User
		* User - Stick Figure
		* Action - Oval
		* Includes (reusable modules) - Dotted line ending in arrow between actions with << includes >>
			- Example: Inserting a bank card so we can deposit or withdraw cash
		* Extends (extra actions on certain conditions) - Dotted line ending in arrow between actions with << extends >>
			- Example: Incorrectly entered PIN
		* Generatisation/Specialisation (Parent/Child) - Solid line with triangle style arrow at end
			- Example: "Business manager" is a specialisation of "Employee"

- Use Case Descriptions
	+ Template
		* Case Name
		* Case ID
		* Stakeholders/Goals
		* Description
		* Actors
		* Trigger (cause)
		* Events
			- Normal flow
			- Sub-flow
			- Exceptional flow
	+ Determine use cases?
		* Identify actors
		* Define actor actions, these become use cases
	+ Describe use cases?
		* Normal events done by actor
			- Example: User does _something_
		* High level ONLY
		* ONLY DESCRIBE ACTIONS NOT BACKEND ACTIONS

- UML Classes
	+ ALL BOXES ARE OPTIONAL
	+ Template
		* Top box: Class name
		* Middle box: Attributes (variables)
		* Lowest box: Operations (functions)
	+ Prefixes for attributes/operations
		* `-` Private
		* `+` Public
		* `#` Protected
	+ Join boxes using relations (solid line no arrow), 1-to-1, one-to-many, etc called multiplicity
		* Defined on both sides
			- 1..1 _(one to one)_
			- 0..* _(many to many)_
			- 0..1 _(zero to one)_
			- 2,4 _(either two or four)_
		* Role names on either side (optional)
			- Example: Person - Company, _employee_ works for _employer_
		* Qualifier
			- In a box attached to the left side, attribute to distinguish between different objects, such as file type in terms of files in a directory.
	+ There are also generalisations using triangle at end of line.
		* Example: Mailbox class has in, out, rubbish, general connected together and to Mailbox via a generalisation.
	+ Object Diagrams
		* Object Symbol
			- INSTANCE OF AN OBJECT, SAVED LIKE A PROGRAM STATE
			- Uses dotted line with arrow from Instance to Class
	+ Links and associations
		* Link is an instance of an association
		* Association - Objects need to communicate (default)
			- Has-A, example Driver drives * _(many)_ Car
			- Diamond at LEFT SIDE (HAS A)
				+ Example: Car has Passengers, diamond on car side, continued on solid line attached to passenger
		* Aggregation - One object part of another object
			- Same as specialisation, but with diamond on PARENT (UNFILLED)
		* Inheritance - One object is a more specialized version of another object
			- 
		* Composition (x is composed of y)
			- Diamond on PARENT, FILLED
		* Navigability
			- Arrow head on association _(as above)_, means a class knows about another (instead of it being inherited)
		* Inheritance (x IS A y)
			- Same as always, unfilled triangle pointed towards parent

- Structure modelling
	+ Used during analysis/design to understand the problem from a business perspective.
	+ 

---

# Lecture 5



---

# Lecture 6



---

# Lecture 7



---

# Lecture 8



---

# Lecture 9



---

# Lecture 10



---

# Lecture 11



---

# Lecture 12



---
