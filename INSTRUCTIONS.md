# ICS4U OOP Design Project

## Overview
In this project, you'll demonstrate your understanding of **Object-Oriented Programming (OOP)** by designing and implementing a Java-based system of your choice. This system should include clear object relationships, encapsulation, and class responsibility separation. Your focus should be on **good design, not excessive scope**.

A successful project:
- Has a clean, scalable structure
- Uses OOP principles: **encapsulation, aggregation, inheritance**
- Avoids being too large to implement fully and properly

<br>

## Part 1 – Choose a System

Choose a real-world or digital system to model using object-oriented design. This could be something from your everyday life, school, home, or an app/service you use often.

Your system must include **at least three meaningful object types** that interact. Keep it simple and **fully implementable** within our project timeline.

### Example Systems You Could Model

Think about the structures you interact with — not just on your phone or computer, but in real life too. Here are some ideas:

#### Everyday Real-World Systems
- **Shoe closet**: shoes categorized by type, season, or occasion; logic to decide what to wear
- **Kitchen inventory**: ingredients, expiry tracking, recipe suggestions based on what's available
- **Personal library**: books organized by genre/author, lend/return system
- **Toolbox or garage**: tools grouped by function, with checkout or maintenance tracking
- **Morning routine planner**: daily tasks with time estimates and dependency (e.g., breakfast before teeth brushing)

#### School-Based Systems
- **Clubs and events**: students, clubs, meetings, and leadership roles
- **Course enrollment**: students, courses, schedules, prerequisites
- **Classroom seating plan**: desks, students, layout preferences or rotations

#### App-Style Digital Systems
- **Streaming media app**: user list of shows, genres, and recommendations (e.g. Netflix)
- **Music manager**: playlists, songs, artists, user favorites (e.g. Spotify)
- **Food delivery**: menus, orders, restaurants, checkout (e.g. UberEats, DoorDash)
- **Online store**: products, shopping cart, checkout, delivery tracking
- **Social media post**: posts, comments, likes, users
- **Ride-sharing**: drivers, riders, trips, fares (e.g. Uber)

#### Organizational Systems
- **Company hierarchy**: employees, roles, departments, manager-subordinate relationships
- **Library checkout system**: books, borrowers, loans, overdue tracking
- **Project management**: tasks, deadlines, team members, dependencies

> ✅ Good scope: A music playlist system with a few extra features  
> ❌ Too much: Trying to build all of Spotify with podcasts, radio, ads, etc.

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

# Helpful Tips & Resources

## Don’t Just Store Data: Make Your Classes Do Work

In this project, your classes shouldn’t just hold information — they should also **do something meaningful**.

### What's A “Dumb Data Class"?

These are classes that just store data, like this:

```java
public class Shoe {
    private String type;
    private String color;
    private String size;

    // Just getters and setters — no logic!
}
```

This kind of class is **passive**. It doesn't help your system actually *do* anything.

### Writing Classes That DO Things

Good object-oriented design includes **behavior**, not just data. Your classes should have methods that act on their properties or help the system make decisions.

Here are some ideas:

#### Shoe Closet System

Instead of just storing shoes, think about what a shoe or closet can *do*:

**Shoe class**
- `boolean isSuitableForWeather(String weather)`
- `boolean matchesOutfit(String outfitColor)`
- `void wear()` — mark this shoe as worn today

**Closet class**
- `Shoe suggestShoe(String weather, String occasion)`
- `List<Shoe> getAllUnwornShoes()`

The bottom line: **Don’t just describe objects — make them act**.

Ask yourself:
> What should this object know?  
> What should this object be able to do?

If your answer is "just store data", dig deeper.

<br>

## Assessment Rubric (Total /46)

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
