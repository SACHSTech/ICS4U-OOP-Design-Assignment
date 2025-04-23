# ICS4U OOP Design Project

## Overview
In this project, you'll demonstrate your understanding of **Object-Oriented Programming (OOP)** by designing and implementing a Java-based system of your choice. This system should include clear object relationships, encapsulation, and class responsibility separation. Your focus should be on **good design, not excessive scope**.

A successful project:
- Has a clean, scalable structure
- Uses OOP principles: **encapsulation, aggregation, inheritance**
- Avoids being too large to implement fully and properly

<br>

## Part 1 – Choose a System

Choose a real-world or digital system that can be modeled with **at least three interrelated object types**. Here are some sample systems:

- Playlist and Song organization in a music app
- Students, Clubs, and Meetings in a school
- Food delivery service: Menus, Orders, Customers
- Online store with Products, Cart, and Orders
- Social feed: Posts, Comments, Likes

**Limit your scope** to something you can fully build within the timeline. More classes does not mean a better mark — deeper, cleaner class design is what earns marks.

> ✅ Good scope: A playlist with songs, plus basic metadata and playback features  
> ❌ Poor scope: All of Spotify with podcasts, AI suggestions, ads, user profiles

<br>

## Part 2 – Class Design & UML Diagram

Use diagrams.net to draw a **UML class diagram** of your system. Include:
- Class names
- Instance variables (with types)
- Methods (with return types + parameters)
- Relationships (aggregation, inheritance)

Follow our [UML house style](https://github.com/davecheng-tech/Random-Notes/blob/main/object-oriented-programming/uml-class-diagrams.md). Add your diagram (PNG format) and a short project description to your `README.md`.

> ✅ Good UML: Shows reusable, abstract class like `Media` with `Song`, `Podcast` as subclasses  
> ❌ Bad UML: Every class has only getters/setters, no useful logic or relationships

<br>

## Part 3 – Class Implementation

Translate your UML into Java code. Your classes must:

- Follow **encapsulation**: use `private` variables, and `public` getters/setters
- Use helper methods to avoid long `main()` functions
- Implement inheritance and method overriding where logical
- Keep data types, naming, and responsibilities clean and consistent

Avoid “dumb data classes” — your classes should **do things**, not just **store things**.

<br>

## Part 4 – Main Program Demonstration

Write a `Main.java` file that **instantiates your classes** and demonstrates how your system works. You must show:

- Objects being created and used
- Relationships between objects (e.g., adding students to a club)
- System logic (e.g., calculating averages, removing from a list, printing summaries)

> ✅ Level 4: Also includes **user interaction** like keyboard input or menu choices  
> ❌ Level 2: Just prints object attributes one after another

<br>

## Rubric (Total /46)

| **Criteria**                       | **Level 4** | **Level 3** | **Level 2** | **Level 1** |
|-----------------------------------|-------------|-------------|-------------|-------------|
| Object-Oriented Design (12 pts)   | 3+ classes, aggregation + inheritance | 3 classes + aggregation | 3 classes, weak relationships | Limited design or unclear |
| UML Diagram (6 pts)               | All classes, relationships, methods & variables shown clearly | Mostly accurate | Some missing structure | Diagram unclear or incomplete |
| Class Implementation (10 pts)     | Fully implemented, encapsulated, clean | Mostly functional | Partial implementation | Errors or unclear logic |
| Main Program (10 pts)             | Instantiates all classes, shows relationships, includes input | Demonstrates relationships | Some relationships shown | Minimal or unclear demo |
| Programming Style (4 pts)         | Proper formatting, naming, comments, javadocs | Mostly good style | Some issues | Poor readability |
| Version Control (4 pts)           | Frequent commits, good README, clean GitHub repo | Moderate commits | Few commits | Poor version tracking |

<br>

## Suggested Project Timeline

Use the guide below to pace yourself and ensure you're making steady progress.

| **Task**                        | **What You Should Do**                                                                 | **Suggested Time** |
|--------------------------------|----------------------------------------------------------------------------------------|---------------------|
| **1. Choose a System**         | Pick a real-world or app-based system. Identify 3+ object types that interact.        | 1 class             |
| **2. Design & UML Diagram**    | Define your classes, relationships, and draw a UML diagram using diagrams.net         | 1–1.5 classes       |
| **3. Implement Classes**       | Write Java classes: private variables, constructors, methods, getters/setters         | 2 classes           |
| **4. Add Relationships**       | Implement inheritance, aggregation (e.g., collections of objects)                     | 1.5 classes         |
| **5. Write Main Program**      | Simulate your system in `Main.java`. Instantiate and connect your objects.            | 1.5 classes         |
| **6. Add User Interaction**    | Add keyboard/menu input to reach Level 4 (optional but recommended)                    | 1 class             |
| **7. Final Polish & GitHub**   | Write your README, upload UML diagram, push final commits to GitHub     | 0.5–1 class         |

Stay on pace. Ask for help early if you're falling behind. A well-scoped, complete system will always earn more than an overly ambitious one that doesn’t work or is poorly implemented.

<br>

## Checklist Before Submission

- [ ] System is realistic, scoped, and implementable
- [ ] At least 3 meaningful object types
- [ ] UML diagram included and follows house style
- [ ] All classes implemented with encapsulation
- [ ] Main program demonstrates class use and relationships
- [ ] README includes system description and PNG diagram
- [ ] Code pushed to GitHub with clear commit history
