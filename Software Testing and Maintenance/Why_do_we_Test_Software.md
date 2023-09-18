# Why Do We Test Software?

## Software Faults, Errors & Failures

Software Fault 
: A static defect in the software

Software Failure 
: External, incorrect behavior with respect to the requirements or other description of the expected behavior

Software Error 
: An incorrect internal state that is the manifestation of some fault

Faults in software are equivalent to design mistakes in hardware. Software does not degrade

![Alt text](<../Images/Software testing/fault.png>)

## Validation & Verification (IEEE)

Validation 
: The process of evaluating software at the end
of software development to ensure compliance with
intended usage

Verification 
: The process of determining whether the
products of a given phase of the software development process fulfill the requirements established during the previous phase

## Testing Goals Based on Test Process Maturity

### Level 0 Thinking
- Testing is the **same** as debugging
- Does not distinguish between incorrect **behavior** and mistakes in the program
- Does not help develop software that is **reliable** or **safe**

### Level 1 Thinking
- Purpose is to show **correctness**
- Correctness is **impossible** to achieve
- What do we know if **no failures**
- **Test engineers** have to:
    - Strict goal
    - Real stopping rule
    - Formal test technique
    - Test managers are **powerless**

### Level 2 Thinking
- Purpose is to show **failures**
- Looking for failures is a **negative** activity
- Puts testers and developers into an **adversarial** relationship

### Level 3 Thinking
- Testing can only show the **presence of failures**
- Whenever we use software, we incur some **risk**
- Risk may be **small** and consequences unimportant
- Risk may be **great** and consequences catastrophic
- Testers and developers cooperate and **reduce risk**

### Level 4 Thinking
- Testing is only **one way** to increase quality
- Test engineers can become **technical leaders** of the project
- Primary responsibility to **measure and improve** software quality
- Their expertise should **help the developers**

## Cost of Not Testing
- Testing is the **most time consuming** and expensive part of software development
- Not testing is even **more expensive**
- If we have too little testing effort early, the cost of testing **increases**
- Planning far testing after development is **prohibitively** expensive

>Summary:
>A tester's goal is to eliminate faults as early as possible:
>- Improve quality
>- Reduce cost
>- Preserve Consumer satisfaction