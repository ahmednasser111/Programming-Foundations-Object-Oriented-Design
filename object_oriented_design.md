# Programming Foundations: Object-Oriented Design
### LinkedIn Learning Course by Simon Allardice

## Why do we use object orientation?
* Programs used to be procedural (the program was written as a long procedure)
* As programs became larger, this became difficult to manage. That's when object oriented programming was introduced (80s).
* Large programs were split into objects. Each object represents a different part of the application and each object has its own data & logic, and they communicate with each other.

Other programming paradigms (mainly used in academics):
* logic programming language (Prolog)
* functional programming language (Haskell)

## What is an object?
### Objects have 3 things:
* identity
* attributes
* behavior

Objects in a computer are self contained. 
Identity -> They have an identity separate from other objects. 
Attributes -> information that describes their current state
Behavior -> things they can do

## What is a class? 
A class is a blueprint for an object.
It describes attributes and behaviors.

## 4 Fundamental Ideas in Object-Oriented Programming:
* Abstraction
* Polymorphism
* Inheritance
* Encapsulation

APIE

### What is abstraction?
Abstraction means we focus on the essential qualities of something rather than one specific example.
It also means we can have an idea or concept that is completely separate from any specific instance. 

### What is encapsulation? 
It is restricting access to the inner workings of a class or objects based on that class. Also known as information hiding or data hiding.

Reason for encapsulation: to reduce dependencies between different parts of the application so that a change in one place won't cascade down and require multiple changes elsewhere.

### What is inheritance?
When you create a class based on an existing class so that the child inherits attributes and behaviors from the parent.

### What is polymorphism? 
Polymorphism means many forms.
It lets us do the correct behavior even if what we're working with could take one of many different forms.

Example: + could add 2 integers. It can also concatenate 2 strings.

## Identifying classes in an application
Typical approach: 
* Gather requirements.
* Describe the app.
* Identify the main objects.
* Describe the interactions.
* Create a class diagram.

### 1. Gather requirements
* What does the app need to do?
* What problem are you trying to solve?
* Write this down.

### 2. Describe the app
* build a simple narrative of how people will use the app
  - use cases
  - user stories
* may or may not create a prototype

### 3. Identify the main objects
* use stories and descriptions from step 2 to identify the most important things/ideas of the app. Many of these things will become classes.

### 4. Describe the interactions
* formally describe the interactions between objects
  - Example: our customer needs to open a bank account.
  - This helps in identifying what methods will be needed
* This could be done with a sequence diagram

### 5. Create a class diagram
* a visual representation of the classes you need
* in interative approach, theses steps are revisited and refined throughout the development process

## Defining requirements
Functional requirements: what does it do?
* features/capabilities

Non-functional requirements: what else?
* help
* legal
* performance
* support
* security

Application must ...

FURPS/FURPS+
* Functional requirements
* Usability requirements
* Reliability requirements
* Performance requirements
* Supportability requirements
+ Design requirements, Implementation requirements, Interface requirements (refers to any external system you need to interface with), Physical requirements

## Use cases
Use cases need at least 3 things: 
* Title: what is the goal?
* Actor: who desires it?
* Scenario: how is it accomplished?

### Use case title
Short phrase, active verb
* register new member
* transfer funds
* purchase items

### Use case actor
Could be a person or external system
* user
* customer
* member
* admin
* ACMESystem

Identifying use case actors:
* Does your app need to interact with other computer systems or other organizations?
* Do you need to distinguish between roles or security groups? 
  - visitor, member, admin, owner

For a use case, use active voice. Omit needless words. 

Use case prompts: 
* Who performs system administration tasks?
* Who manages users and security?
* What happens if the system fails? 
* Is anyone looking at performance metrics or logs?

### Use case scenario
Different formats: 
* paragraph
* list of steps
* fully dressed use case templates (often exist as PDFs)
  - requiring this level of detail can kill a project

Work one or two days per iteration on use cases.

### Use case diagram
It's typically a diagram of several use cases and multilple actors at the same time. Gives us an overview and allows us to see how they interact.

## User Story
Simpler and shorter than use case.
Usually 1-2 sentences.
Describes a small scenario from the user's perspective.

Typical format: 
* As a (type of user or role)
* I want (the goal)
* so that (the reason or benefit)

Example: 
* As a user
* I want to sort entries by date
* so that I can find the most recent content.

## Differences between user stories and use cases
### User stories:
* short - one index card
* one goal, no details
* informal
* "placeholder for conversatio"

### Use cases: 
* long - document
* multiple goals & details
* casual to very formal
* "record of conversation"

You can use user stories, or use cases, or both.

## Create a conceptual model of the app
* Identify objects
  - Start making a list of possible objects (use nouns from your use cases)
* Identify class relationships
  - not the same as SQL schema
* Identify class responsibilities
  - look for verbs in your use cases
  
## CRC cards
Create a CRC card for each class. The CRC card has 3 sections: 
* C: name of the class (at top, underlined)
* R: responsibilities of the class
* C: collaborators (other classes it interacts with)

## Inheritance, Aggregation, Composition
Inheritance describes an "is a" relationship.
Aggregation describes a "has a" relationship. 
* A customer has an address.
* A car has an engine.
* A bank has many bank accounts.
Composition is a more specific form of aggregation. 
* With composition there is a dependency. It implies ownership. 
  - Example: a document has many pages. If the document object gets deleted so should all the page objects.
  
## UML (Unified Modeling Language)
Types of UML diagrams seen in the course:
* class
* use case
* object
* sequence

UML Tools:
* Diagramming tools
  - Visio, OmniGraffle
* Web-based diagramming
  - gliffy.com, creately.com, lucidchart.com
* Programming tools: IDE based
  - Visual Studio, Eclipse with UMLTools
* Commercial Products
  - Altova, UModel, Sparx Enterprise Architect, Visual Paradigm
* Open-Source
  - ArgoUML, Dia
  
## Design Patterns
Design patterns are well tested solutions to common issues and problems we run into in software development.

Design Patterns book by the Gang of Four includes 23 design patterns.

### Singleton Design Pattern
Used when you only want to create one object of a particular class
* We want to ensure a class has only one instance
* We want one way of accessing it

### Memento Design Pattern
* handles "undo" in an object
* does not violate encapsulation
* has 3 classes: originator, caretaker, memento






