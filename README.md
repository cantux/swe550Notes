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

Focus
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

### Six Sigma

### Measurement theory

### Reliability

### Validity

### Types of validity

### Causality

### Software quality metrics

### Defect rate

### Defect density

### Quality tools

### Reliability Growth Model

### PTR Arrival mode

### Cyclomatic complexity

### CK OO metrics

### Coverage

