# swe550Notes
Decided to dump things that seem relevant(keeping in mind the importance to the instructor). A summary will be created based on this; will also help reiterate.

## Keywords:

### Quality definition

**Small q(functional quality):** Software functional quality reflects how well it complies with or __conforms__ to a given design
* Measurements are taken regularly to determine conformance to those requirements. The non-conformances are regarded as defects
* Measured by
  * **Defect rate**
    * number of defects per million lines of source code
    * per function point, or other unit
  * **Reliability**
    * number of failures per n hours of operation
    * mean time to failure
    * the probability of failure free operation in a specified time
    
**Big Q(structural quality):** Fitness for use (relative to needs)
* Takes customers' requirements and expectations into account
  * Customer satisfaction: percent satisfied
* Includes other attributes
  * product quality
  * process quality
  * customer satisfaction
  * project business objectives
  * organizational objectives

Process quality vs. Product Quality 

**Quality metrics and models are our focus**

**“Optimize” quality (not maximize)**

### Quality engineering

* Quality engineering is about effective ways to achieve project objectives. 
* Processes and metrics are enablers to achieve these objectives. 
* Metrics Interpretation is the real value added by the quality engineer.

### Software process
**Process Model:** Methodology
1- A body of methods, rules, and postulates (accepted theory or statement) employed by a discipline. 
2- A particular procedure or set of procedures

**Common Process Models**

* Waterfall
  * Encourages requirements gathering, ordered stages, and documentation 
  * Divide and conquer approach
  * Deliverables at each stage
  * Entry/Exit criteria for each stage
  * Feedback between stages
  * Emphasis on documents  
  * Clearly defined **stages**:
    * Requirements
    * Design
      * Architecture: The **structure** of the **components** of a _program system, their relationships, and principles and guidelines_ **governing** their _design and evolution_ over time. 
      * High-Level Design (HLD) 
        * Develop external functions and interfaces
        * Ensure components fit into system/product structure (feedback to Architecture stage) 
        * Ensure external functions can be accomplished (feedback to Requirements stage) 
      * Low Level Design (LLD) 
        * Identify parts, modules, macros, include files, etc. that will be written or changed
        * Finalize detail level of design
        * Verify changes in HLD (feedback to HLD)
        * Verify correctness/completeness of HLD (feedback to HLD) 
    * Code
    * Test
      * Unit Test
        * Verify code against LLD/HLD 
      * Component Test
        * Functionality
        * Intra-component (module) interfaces
        * Error recovery
        * Messages
        * Concurrency (multi-tasking)
        * Shared Resources
        * Existing functionality (regression) 
      * System-Level Test: Four portions: System Test, Regression Test, Performance, Usability
        * System Test
          * Test concurrency
          * Stress test
          * Test overall system stability and completeness 
        * Regression Test
          * Test original (unchanged) functions
        * Performance Test
          * Validate performance of system/product against requirements
          * Record performance metrics
          * Establish baselines (I.e. benchmark)
        * Usability Test
          * Test for usability requirements 
      * Goal of Testing
        * **Verification:** 
          * Verify that the system/product we built meets all of the user requirements for usability, performance, reliability, etc.
          * Verify that the intrinsic quality is high and that standards have been met.
        * **Validation:**
          * Validate that the requirements that drove the process were correct
    * Maintenance
    * Waterfall Adv:
      * Better than an adhoc approach
      * Process, requirements, entry/exit criteria, designs are all documented 
    * Waterfall Disadv:
      * Assumption that requirements will not change
      * Heavy emphasis on documents
      * Performance problems detected late in cycle
      * Rework is costly
      * Feedback is not formalized 
      
* Prototyping: Designed to deal with changing or unknown customer requirements. 

  * **Prototype**: is a partial implementation of the product expressed either logically or physically with all external interfaces presented. 
  * Prototyping steps:
    * Requirements gathering and analysis
    * Quick design
    * Build prototype
    * Customer evaluation
    * Refinement of design and prototype (and requirements)
    * Decision: Iterate or accept 
  * **Key to success:** Quick turnaround and inexpensive
  * Prototype **types**:
    * **Rapid Throwaway:** “quick and dirty” approach 
      * Good for:
        * High-risk projects
        * Complex problems
        * Performance concerns
    * **Evolutionary:** Each iteration evolves (refines) prototype
      * Some requirements are known
      * May or may not become final product 
  * Disadvantages
    * Hard to know when to stop
    * Could be costly
    * Tempting to use prototype as product (in throwaway approach) 
    
* Spiral: Refinement of the Waterfall Model. Focus is on **Risk Management** and **prototyping**. **Prototyping** is applied to the **high-risk areas**  

* Iterative
  * Start with subset of requirements and develop a subset of the product to meet these requirements. 
  * Non-iterative portion like Waterfall Model, Iterative portion like Prototyping Model 
  * Test suite developed at each iteration
  * Each iteration is verified and validated 
  
* Object-Oriented: Oops, mind rejects to learn this.
* Cleanroom: Do you even?

### Defect prevention
Defect Prevention Process: continually improving a software development process 

Three main steps:
* Analyze existing defects or errors to trace the root cause
* Suggest preventative actions to eliminate the
defect root cause
* Implement the preventative actions 

Four key elements:
* **Causal analysis meeting**: two-hour brainstorming sessions conducted by technical teams at the end of each stage of the development process. analyze defects for each stage of the development process, identify root cause, identify prevention actions, look for trends
* **Action team**: prioritize and implement action items
* **Stage kickoff meeting**: level setting, emphasis on quality improvement through action items and process improvements, pitfalls identified and discussed 
* **Action tracking and data collecting**: record all problems, root causes, and actions (and action status) 

DPP can be used with any development model, but may be more effective with some (I.e. iterative) 

### Quality system
An organization uses quality systems to control and improve the effectiveness of the processes used to deliver a quality product or service

A Quality System is a set of formal and informal practices and processes that focus on the following to achieve organizational outcomes:
* Customer needs
* Leadership vision
* Employee involvement
* Continual improvement
* Informed decision making based on real-time data
* Mutually beneficial relationships with external business partners 
 
### Quality framework

A quality system framework is a coherent set of objectives, policies, and practices for managing quality in an organization 
As a framework, it provides the essential elements of a quality system
  * The elements are expected to be tailored and expanded for a given organization and situation
  * The framework emphasizes what needs to be done and why, without prescribing how 
  
* A quality system framework can help an organization to: 
  * Review their current quality activities
  * Identify quality system elements that may already exist
  * Identify additional elements needed to implement a quality system 
* Use a quality system framework for external assessment and validation 
  * Objective criteria for assessing quality processes 
  * Often required to be “in business”
    * Cannot bid on a contract if you are not certified
    * Use as a marketing tool—Certified Seal of Approval
    
### Quality principle
Edward Deming:
* Continuously improve product, service, and process
  * Result: continuously decreasing cost
* Don’t depend on detecting defects; Prevent them
* Don’t focus on initial cost, instead minimize total cost in a long-term relationship of loyalty and trust
* Drive out fear, so that everyone may work effectively for the company 
* Break down barriers between departments, roles, and
disciplines
* Eliminate defect and productivity targets – management by
numbers
  * Substitute leadership
  * Enable pride of workmanship 

TQM:
* Quality can and must be managed
* Customer focus; Everyone has a customer and is a supplier
* Processes, not people are the problem
* Every employee is responsible for quality
* Problems must be prevented, not just fixed
* Quality must be measured
* Quality improvements must be continuous
* The quality standard is defect free
* Goals are based on requirements, not negotiated
* Life cycle costs, not front end costs
* Management must be involved and lead
* Plan and organize for quality improvement

## Process Maturity Frameworks
Attempt to measure implementation maturity of a software development process (i.e. how well is it executed), and analyze the quality management systems in place

---

The following two are not given as keywords and will be ommitted on the summary:

### Software Productivity Research (SPR) assessment 
* Based on 400 question questionnaire. Questions are rated 1-5, and overall process rating is expressed on 1-5 scale
* While SEI's questions focus on software organization structure and software process SPR Questions focus on
  * Strategic corporate issues
  * Tactical project issues
    * Quality, Productivity, Customer satisfaction 

### Total Quality Management (TQM)
* A philosophy and practices for improving quality
* Build an organization-wide quality culture, focusing on providing customers with the products and services that satisfy their needs
* Do it right the first time; eliminate defects and waste

---

### ISO 9000
* Oriented towards assessment and certification 
* Heavy focus on processes and evidence of compliance (documentation)
* Complementary to other quality management frameworks
* Formal Audit performed 

* Focus
  * Process quality
  * Process Implementation 

* Product Metrics Goals
  * Collect data and report values on regular basis
  * Identify current metric performance level
  * Take action if performance level is unacceptable
  * Establish improvement goals
* Process Metrics Goals
  * Determine if quality objectives are being met
  * Track adherence to process model and methods
  * Track defect prevention effectiveness 

### MBQNA Malcolm Baldrige National Quality Award
Very broad applies to all businesses.

* 28 examination items 1000 possible points awarded Scoring is based on three evaluation dimensions:
  * Approach - methods used to address the item
  * Deployment - extent to which the approach is applied
  * Results - outcomes and effects 
* To be the MBNQA winner, the four basic elements of the award criteria must be evident:
  * Driver: The leadership of the senior executive management team.
  * System: The set of well-defined and well-designed processes for meeting the company's quality and performance requirements.
  * Measure of progress: The results of the company's in-process quality measurements (aimed at improving customer value and company performance).
  * Goal: The basic aim of the quality process is the delivery of continuously improving value to customers.

### SEI CMM Software Engineering Institue Capability Maturity Model

* Level 1: Initial: Characteristics: Chaotic—unpredictable cost, schedule, and quality performance.
* Level 2: Repeatable Characteristics: Intuitive—cost and quality highly variable, reasonable control of schedules, informal and ad hoc methods and procedures. 
  * key process areas (KPA):
    * Requirements management
    * Software project planning and oversight
    * Software subcontract management
    * Software quality assurance
    * Software configuration management
* Level 3: Defined: Characteristics: Qualitative—reliable costs and schedules, improving but unpredictable quality performance. The key elements to achieve this level of maturity follow:
  * Organizational process improvement
  * Organizational process definition
  * Training program
  * Integrated software management
  * Software product engineering
  * Intergroup coordination
  * Peer reviews 
* Level 4: Managed: Characteristics: Quantitative—reasonable statistical control over product quality. The key elements to achieve this level of maturity follow:
  * Process measurement and analysis
  * Quality management 
* Level 5: Optimizing: Characteristics: Quantitative basis for continued capital investment in process automation and improvement. The key elements to achieve this highest level of maturity follow:
  * Defect prevention
  * Technology innovation
  * Process change management
  
Following is a list of metrics-related topics addressed by the questionnaire.
* Profiles of software size maintained for each software configuration item over time
* Statistics on software design errors, Statistics on software code and test errors
* Projection of design errors and comparison between projected and actual numbers
* Projection of test errors and comparison between projected and actual numbers
* Measurement of design review coverage, Measurement of test coverage
* Tracking of design review actions to closure, Tracking of testing defects to closure
* Database for process metrics data across all projects
* Analysis of review data gathered during design reviews
* Analysis of data already gathered to determine the likely distribution and characteristics of the errors in the remainder of the project
* Analysis of errors to determine their process-related causes
* Analysis of review efficiency for each project

Several questions on defect prevention address the following topics:
* Mechanism for error cause analysis
* Analysis of error causes to determine the process changes required for error prevention
* Mechanism for initiating error-prevention actions

### Six Sigma
* Focuses on people rather than roles as the solution
* Has metrics and measured improvement as core principles 

### Measurement theory
Basic measurement theory steps
* Proposition
* Definition
* Operational Definition
* Metric definition
* Hypothesis definitions
* Testing and metric gathering
* Confirmation or refutation of hypothesis

* Front end SW process = design through unit test
* Back end SW process = integration through system test 

How measurements are classified and compared(low to high):
* Nominal Scale
  * Jointly exhaustive (all items can be categorized)
  * Mutually exclusive (only one category applies) 
  * Example: Categories of SW dev: Waterfall, Spiral, Iterative, OO. Does not imply that Waterfall is ‘better/greater’ than Spiral 
* Ordinal Scale
  * Like nominal except comparison can be applied but we cannot determine magnitude of difference 
* Interval Scale
  * Like ordinal scale, except now we can determine exact differences between measurement points
  * Can use addition/subtraction expressions 
* Ratio Scale 
  * Can use multiplication and division
  
Measures are ways of analyzing and comparing **data** to extract meaningful **information**. 

Basic measures
* Ratio
* Proportion
* Percentage
* Rate 

### Reliability
Consistency of a number of measurements taken using the same measurement method on the same subject 

Example: 

If an operational definition of a body height measurement of children (e.g., between ages 3 and 12) includes specifications of the time of the day to take measurements, the specific scale to use, who takes the measurements (e.g., trained pediatric nurses), whether the measurements should be taken barefooted, and so on, it is likely that reliable data will be obtained.

* Reliability can be expressed in terms of the size of the standard deviations of the repeated measurements. When variables are compared, usually the index of variation (IV) is used. IV is simply a ratio of the standard deviation to the mean:
  * IV = Standard Deviation / Mean
* The smaller the IV, the more reliable the measurements

### Validity
Validity is whether the measurement really measures what is intended
to be measured 

Example:

For example, a new bathroom scale for body weight may give identical results upon five consecutive measurements (e.g., 160 lb.) and therefore it is reliable. However, the measurements may not be valid; they would not reflect the person's body weight if the offset of the scale were at 10 lb. instead of at zero. 


### Types of validity

*Construct Validity - validity of a metric (operational measurement) to represent a theory 
*Criterion-related (predictive) Validity - validity of a metric to predict a theory or relationship
*Content Validity - the degree to which a metric covers the meaning of the concept 

### Causality
Identification of cause and effect relationships in experiments

* Validity and Reliability represent measurement quality
* Correlation and Causality are goals of measurement

### Software quality metrics

Product Metrics: size, complexity, design features, performance, and quality level 
Process Metrics: effectiveness of defect removal, pattern of testing defect arrival, and response time of fixes 
Project Metrics: number of developers, cost, schedule, productivity, etc. 

* End-Product Metrics
  * Mean Time to Failure (MTTF)
  * Defect Density
  * Problems per User Month (PUM)
  * Customer Satisfaction
* In-Process Project Metrics
  * Defect density during machine testing
  * Defect arrival patterns during machine testing
  * Phased-based defect removal
  * Defect removal effectiveness
  
### Defect rate
number of estimated defects 

Defect count / KLOC, time etc.

### Defect Removal Effectiveness
(Defects removed in the phase / defects latent in product) x 100% 

* Process quality metrics - focus on quality and effectiveness of the process.
  * Defect density during machine testing
  * Defect arrival rate during machine testing
  * Phased based defect removal
  * Defect removal effectiveness
* Metrics for Software Maintenance
  * Fix backlog and backlog management index
  * Fix response time and fix responsiveness
  * Percent delinquent fixes
  * Fix quality 

Metrics that are taken into account:

Defect origin
Stage where the defect was found
Defects Entry
Defects Injected
Defects Total
Defects Removed by Stage
Defects Latent

### Quality tools
1- Checklist (or Check Sheet)
2- Pareto Diagram: 80-20
3- Histogram
4- Scatter Diagram: Correlation
5- Run Chart: metric/time: find trends
6- Control Chart
7- Cause-Effect Diagram 

### Reliability Growth Model

### PTR Arrival mode

### Cyclomatic complexity

### CK OO metrics

### Coverage

