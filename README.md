# swe550Notes

## Keywords:

### Quality definition

Small q(functional quality): Software functional quality reflects how well it complies with or __conforms__ to a given design
* Measurements are taken regularly to determine conformance to those requirements. The non-conformances are regarded as defects
* Measured by
  * **Defect rate**
    * number of defects per million lines of source code
    * per function point, or other unit
  * **Reliability**
    * number of failures per n hours of operation
    * mean time to failure
    * the probability of failure free operation in a specified time
    
Big Q(structural quality): Fitness for use (relative to needs)
* Takes customers' requirements and expectations into account
  * Customer satisfaction: percent satisfied
*  Includes other attributes
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
    
* Prototyping
  * Rapid Throwaway
  * Evolutionary
* Spiral
* Iterative
* Object-Oriented
* Cleanroom 

### Defect prevention

### Quality system

### Quality framework

### Quality principle

### MBQNA

### ISO 9000

### Six Sigma

### CMM

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

