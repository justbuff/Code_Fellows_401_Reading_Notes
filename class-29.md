# Threat Modeling

A threat model is a structured representation (capturing, organizing, and analyzing) of all the information that affects the security of an application. Applied to software, it enables informed decision-making about application security risks. In addition to producing a model, typical threat modeling also produces a prioritized list of security improvements to the concept, requirements, design, or implementation of an application.

A threat model typically includes:

- Description of the subject to be modeled

- Assumptions that can be checked or challenged in the future as the threat landscape changes

- Potential threats to the system

- Actions that can be taken to mitigate each threat

- A way of validating the model and threats, and verification of success of actions taken

Threat modeling is best applied continuously throughout a software development project. Updating threat models is advisable after events such as:

- A new feature is released

- Security incident occurs

- Architectural or infrastructure changes

The following framework can help to organize threat modeling:

1. Assess Scope

2. Identify what can go wrong

3. Identify countermeasures or manage risk

4. Assess your work


# STRIDE Security Threat Model

One common threat modeling approach is the STRIDE framework, which has six areas of focus:

1. Spoofing- The security of your systems depends upon trust in the other party’s identity. A threat to this trust is spoofing; when someone claims to be a person or system they are not.

2. Tampering- Even if you feel confident in your authentication security, trust must extend to all systems you touch. Data is especially susceptible to threats of tampering, but physical machines or hardware may also be vulnerable.

3. Repudiation- Repudiation threats take aim at your auditing and tracing, ensuring that bad behavior cannot be proven.

4. Information Disclosure- There are any number of methods that can be used to access private data and can impact a single user, multiple people, or be specific to a business itself.

5. Denial of Service- In networking, this can mean overloading a system with incoming requests, making it impossible for users to connect.

6. Elevation of Privilege- The attacker not only claimed to be a valid user, but one with an expanded role.
