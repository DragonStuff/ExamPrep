# Revision

CSIT314, the last --4 subject. Thank goodness.

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
	+ Analysis - Logical structure, not concerned with infrastructure or code
	+ Design - Database tables, file formats, data types, concerned with infra and code

- Domain model
	+ Created during analysis
		* Domain model contains key data/elements from problem
		* Common vocabulary between client and dev
		* No implementation details
		* Contains methods and relationships between classes
	+ Identify classes using textual analysis
		* Reading requirements/functional spec
			- Nouns - Classes
			- Verbs - Methods
			- Adjectives - Attributes
		* Be aware of scope
		* Association
			- Any dependency between 2+ classes will be an association
			- Reference from one to another may be an association
			- Verb phrases from the problem may be an association
			- Real world knowledge will lead you to associations
		* Attributes
			- Belonging to the object
		* Operations
			- OR Changes the object (manipulates data)
			- OR Performs a computation
			- OR Monitors the object
	+ Data Dictionary
 		* Paragraph of each object class containing
			- Scope of class
			- Attributes and operations
			- Subclasses that inherit
		* Template
			- Class Name
			- Short description
			- List of attributes
			- List of Operations
				+ Target class
				+ Return value
				+ Description (brief)

---

# Lecture 5

- Agile methods
	- Agile principles
		+ The highest priority is to satisfy the customer through early and continuous delivery of valuable software.
		+ Welcome changing requirements, even late in development. Agile processes harness change for the customer's competitive advantage. 
		+ Deliver working software frequently, from a couple of weeks to a couple of months, with a preference to the shorter timescale.
		+ Business people and developers must work together daily throughout the project.
		+ Build projects around motivated individuals. Give them the environment and support they need, and trust them to get the job done.
		+ The most efficient and effective method of conveying information to and within a development team is face-to-face conversation.
		+ Working software is the primary measure of progress.
		+ Agile processes promote sustainable development. The sponsors, developers, and users should be able to maintain a constant pace indefinitely.
		+ Continuous attention to technical excellence and good design enhances agility.
		+ Simplicity--the art of maximizing the amount of work not done--is essential.
		+ The best architectures, requirements, and designs emerge from selforganizing teams.
		+ At regular intervals, the team reflects on how to become more effective, then tunes and adjusts its behaviour accordingly.

---

# Lecture 6

- Scrum
	+ Characteristics
		* Self-organising
		* SPRINTS!
		* Requirements are user stories in a BACKLOG
		* No specifics
		* Type of Agile
	+ Sprints
		* How progress is made
		* 2-4 weeks
		* Design, coding and testing all occurs in the sprint
	+ Roles
		* Product owner
			- Decide features
			- Decide release date
			- Decide content
			- ROI
			- Prioritises/adjusts features and priority every iteration
			- Accept/Reject work
		* Scrum Master
			- Represents management to project
			- Enforces scrum
			- Enforces productivity
			- Enables cooperation
		* Team
			- 5 to 9 people
			- Cross-functional (programmers, testers, UI, etc)
			- Self organised, may only change members between sprints
	+ Meetings
		* Sprint planning
			- Decide on goal for sprint - (focused task)
			- Tasks are identified and estimated in hours/story points
			- Collaborative (all of the team)
		* Sprint review
			- Review accomplishments
			- Demo
			- INFORMAL (2 hour prep time, no slides)
			- ALL TEAM
		* Sprint retroactive
			- Look at what is/isn't working
				+ Start, stop, continue doing
			- 15-30 mins
			- Every sprint end
			- ALL TEAM including customers
		* Daily scrum meeting
			- 15 minutes, stand up
			- Questions
				+ What did you do yesterday?
				+ What will you do today?
				+ Is anything in your way?
			- Commitment-oriented
	+ Artifacts (key items)
		* Product backlog
			- Item (As x I want to y)
			- Estimated difficulty (STORY POINTS)
		* Sprint backlog
			- Item (Code x, write y)
			- Days of week with hours/story points
			- Any member can add, delete or change
			- Update as work is added, done
		* Burndown charts (of remaining user story points)
			- Burn down in either hours or story points

---

# Lecture 7
- UML modelling 
	+ The “4+1” view 
		* Conceptual
			- Logical
				+ Functionality _(that the system provides to end users)_
				+ Components
					* Class
					* Object
					* Package
					* Composite Structure
					* State Machine
			- Process _(dynamic aspects)_
				+ Components
					* Sequence
					* Communication
					* Activity
					* Timing
					* Interaction Overview
				+ Performance
				+ Scalability
				+ Throughput
		* Physical (represent application compoents as built and deployed)
			- Implementation
				+ Configuration
				+ Management
			- Deployment
	+ Logical view 
		* Class and object diagrams 
		* Packages 
			- Expressed same as Java packages (system.company.component)
			- Each package has many classes
			- Can import from other packages
		* State diagrams 
			- Characteristics
				+ Model dynamic aspects by considering use cases
				+ Behavioral model, states the object goes through
				+ Reacts to external stimuli
			- Features
				+ Set of values/atributes that describe a point in an objects life
			- State
				+ Object states change, for example a student from new to current to former
			- Event
				+ Takes places at a point
				+ Cocurrency supproted
			- FORMAT
				+ State - Rectangle with rounded corners
				+ Initial state - Small filled in circle
				+ Final state - Small filled in cirle with circle surrounding not filled
				+ Event - A text label
				+ Transition between events - Solid line with arrow
					* Source State
					* Trigger (EVENT TRIGGER)
					* Condition (ONLY IF) (optional)
					* Action (ACT ON OBJECT) (optional)
					* Target State
	+ Process view 
		* Sequence diagrams 
			- How objects interact together through MESSAGES
			- Follows process from inception to termination
			- Horizontal and vertical
			- Shows life of object
			- Dotted lines between objects
			- Ends with X
			- Focus of control (sender/reciever) shown by narrow rectangle
			- Simple message SENT shown by SOLID line between focus of control (rectangles) and labelled
			- Simple message RECIEVED shown by DOTTED line between focus of control (rectangles) and labelled
		* Communication diagrams 
			- How objects interact together through METHODS
			- Same as sequence but different style
			- Focus on links between objects
		* Activity diagram 
			- TELLS YOU WHAT HAPPENS BUT NOT WHO DOES WHAT
			- Characteristics
				+ Model workflow on the backend
				+ Analysing a use case
			- PARTS
				+ Initial node
				+ Actions - Rounded rectangle
				+ Control flow - Arrow
				+ Final node - Circle with X (parallel) OR with dot (final all)
				+ ObjectNode - Sharp rectangle with object type
				+ DecisionNode - Diamond with multiple outs using `[]` labels going to other parts of flow
				+ MergeNode - Two diamonds with multiple outs using `[]` labels (one is decision node, one is merge node)
				+ ForkNode - Rectangle, parallel execution
				+ JoinNode - Rectangle, end of parallel execution and continue once both are done
				+ Timed trigger - Hourglass with label
		* SWIMLANES SEPERATE ACTIVITY DIAGRAM HORIZONTALLY WITH NAMES OF ACTORS AT TOP!!!!
		* Interaction Overview Diagrams 
			- SAME FORMAT AS ACTIVITY DIAGRAM
			- ADDS A FUNCTION THAT CONSITS OF AN INTERNAL ACTIVITY DIAGRAM WITH `sd` or `ref` at the top left
			- Sequence
			- Communication
			- Recursion
- DIAGRAM
	+ Deployment view 
		* Deployment diagrams 
			- Models run-time architecture
			- Shows servers and software
			- Node is a 3D box with name, type labels inside underlined
			- Artifact is a rectangle representing a file, executable, document, prototype etc using `<<artifact>>`
			- Association with `<< layer >>` where layer is how it communicates
			- NODES CAN CONTAIN THINGS LIKE ARTIFACTS OR COMPONENTS (:keyboard, :motherboard)
	+ Implementation view 
		* Composite diagrams 
			- Static structure diagram
			- Shows the internal structure of a class and the collaborations that this structure makes possible
			- Methods, parameters and variables via small squares with labels inside of a class
		* Component diagrams 
			- Represents high level classes and services
			- Pieces of software that make up a system
			- One or more classes at runtime
			- Assembly connector like an Eye with protective layer connecting two components

---

# Lecture 8

- Software testing and Test-Driven Development
	- Verification and validation
	- Static verification (software inspection)
	- Dynamic verification (software testing)
	- Test-driven development

---

# Lecture 9

- UML diagrams and RUP
- Rational Unified Process (RUP)

---

# Lecture 10

- Extreme Programming
- Dynamic Systems Development Method

---

# Lecture 11

- DevOps

---

# Lecture 12

- Capability Maturity Model Integration (CMMI) model

---
