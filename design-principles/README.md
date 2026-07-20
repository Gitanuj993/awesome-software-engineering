# Fundamental Software design principles.

```txt
Software design translates the analysis model (requirements) into a design model that can be
implemented. Good design is guided by a set of fundamental principles that help control complexity
and improve quality, maintainability and reusability of software
```

• Abstraction: Focusing on the essential characteristics of a component while suppressing
unnecessary implementation detail. Data abstraction, procedural abstraction and control abstraction
are common forms.

• Modularity: Dividing software into separate, independently developed and testable
modules/components that together satisfy the requirements. Modularity reduces complexity and
eases maintenance.

• Architecture: The overall structure of the software components, their properties, and the
relationships/interactions among them.

• Refinement (Stepwise Refinement): A top-down design strategy in which a program is developed
by successively refining levels of procedural detail, moving from a high-level statement of function to
program statements.

• Refactoring: A reorganization technique that simplifies the design of a component without changing
its function or external behaviour, improving internal structure.

• Design Classes: Identifying a set of classes (user-interface, business-domain, process, persistent,
system classes) that together realize the software.

• Information Hiding: Modules should be designed so that information (data and procedure)
contained within a module is inaccessible to other modules that have no need for such information
— achieved through well-defined interfaces.

• Functional Independence: Achieved by designing modules with high cohesion (a module performs
a single, well-defined task) and low coupling (minimal interdependence between modules). High
cohesion and low coupling lead to software that is easier to develop, test and maintain

