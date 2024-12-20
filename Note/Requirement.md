# Object Oriented Design: Requirements Analysis/Business Modelling

## 1. Case Study Overview
- Focus on Restaurant Booking System
- Coverage across multiple lectures:
  * Requirements analysis
  * Analysis
  * Design
  * Implementation
- Represents one iteration in Unified Process

## 2. Restaurant Booking System Requirements

### Current System Problems
- Manual booking sheet issues:
  * Slow updates
  * Hard to read
  * No data backup
  * Difficult data analysis

### New System Requirements
- Must display similar format as manual system
- Easy data modification
- Immediate updates
- Core functionality for first iteration:
  * Record bookings
  * Modify booking time/table
  * Cancel bookings

## 3. Use Case Modelling

### CRUD Operations
- Create
- Read
- Update
- Delete

### Key Components
1. Actors:
   - Represent different user roles
   - In restaurant system:
     * Receptionist (handles advance bookings)
     * Head waiter (manages open restaurant operations)

2. Use Cases:
   - Describe specific tasks
   - Must be understandable by all stakeholders
   - Main use cases identified:
     * Add booking
     * Cancel booking
     * Alter booking

### Use Case Documentation
1. Standard Template Headers:
   - Name
   - Description
   - Actors
   - Triggers
   - Preconditions
   - Postconditions
   - Courses of events
   - Inclusions
   - Data Outcomes

2. Courses of Events Types:
   - Basic course
   - Alternative course
   - Exceptional course

## 4. Use Case Structuring

### Use Case Inclusion
- Shared functionality can be extracted into separate use cases
- Shown with dashed arrows in diagrams
- Example: "Display Bookings" used by multiple other use cases

### Actor Generalization
- Shows relationships between actors
- Indicates shared capabilities
- Represented by inheritance arrows in diagrams

## 5. Domain Modelling

### Key Concepts
- Customers
- Reservations
- Tables
- Walk-ins

### Class Relationships
```
Customer (name, phoneNumber)
Booking (covers, date, time)
Table (places)
WalkIn extends Booking
```

## 6. Glossary Development
- Important for consistent terminology
- Key terms defined:
  * Booking
  * Covers
  * Customer
  * Diner
  * Places
  * Reservation
  * Walk-in

## 7. CRC Modelling
- Class-Responsibility-Collaborators
- Group exercise approach
- Card structure:
  1. Class name
  2. Responsibilities
  3. Collaborators

### Identification Techniques
- Classes: Look for nouns in specifications
- Responsibilities: Look for verbs in specifications

## Best Practices
1. Avoid unnecessary interaction details in use cases
2. Keep user interface details separate from use case descriptions
3. Maintain consistency in terminology
4. Document all possible courses of events
5. Use proper UML notation in diagrams