# Java Collections Set Architecture Challenges

A pure Java project focused on Set data structures, collection operations, mathematical set algorithms, enum-based modeling, and regex-based string processing.

The project demonstrates how `HashSet` and `TreeSet` can be used to manage unique objects, compare task collections, calculate set relationships, and extract unique words from text data.

## Overview

This project includes two main Java collection scenarios:

1. Task assignment analysis using Set operations
2. Unique word extraction and alphabetical sorting from a text source

The main focus is Java collection design, object uniqueness rules, set-based algorithms, enum usage, and string cleanup with regular expressions.

## Tech Stack

* Java
* Maven
* Java Collections Framework
* HashSet
* TreeSet
* Enum types
* Regex
* Object-oriented design

## Core Concepts

* Java Set architecture
* `HashSet` usage
* `TreeSet` usage
* Object uniqueness rules
* `equals()` and `hashCode()` logic
* Enum-based domain modeling
* Union operation
* Intersection operation
* Difference operation
* Regex-based text cleanup
* Unique word extraction
* Alphabetical sorting

## Scenario 1: Task Assignment Analysis

The project models a simple task assignment system for a team with three employees:

* Ann
* Bob
* Carol

Each employee has a set of assigned tasks. The system analyzes task ownership and answers questions such as:

* Which tasks exist across all employees?
* Which tasks belong to a specific employee?
* Which tasks are unassigned?
* Are there tasks assigned to more than one employee?
* What are the overlapping or different tasks between employees?

## Domain Model

### Task

The `Task` class represents a work item.

Main fields:

* `project`
* `description`
* `assignee`
* `priority`
* `status`

A task's uniqueness is determined by the combination of:

```text
project + description
```

### Priority Enum

```text
HIGH
MED
LOW
```

### Status Enum

```text
IN_QUEUE
ASSIGNED
IN_PROGRESS
```

### TaskData

The `TaskData` class stores task collections for different employees:

* `annsTasks`
* `bobsTasks`
* `carolsTasks`
* `unassignedTasks`

It also provides methods to retrieve and compare task sets.

## Set Operations

### Union

Combines multiple sets into one collection of unique tasks.

```text
A ∪ B
```

### Intersection

Finds common elements between two sets.

```text
A ∩ B
```

### Difference

Finds elements that exist in one set but not in another.

```text
A - B
```

## Scenario 2: Unique Word Extraction

The second part of the project focuses on text processing.

The `StringSet` class includes a static method:

```java
findUniqueWords()
```

This method processes a long text source and performs operations such as:

* Removing punctuation characters
* Cleaning text content
* Splitting text into words
* Finding unique words
* Sorting words alphabetically
* Returning the final unique word collection

## Features

* Team task collection modeling
* Set-based task comparison
* Union, intersection, and difference operations
* Unique task detection with object equality
* Enum-based task priority and status modeling
* Regex-based punctuation cleanup
* Unique word extraction from long text
* Alphabetical sorting with Set structures
* Pure Java implementation without external business frameworks

## Project Structure

```text
src/
 └── main/
     └── java/
         └── org/example/
             ├── entity/
             │   ├── Task.java
             │   ├── TaskData.java
             │   ├── Priority.java
             │   ├── Status.java
             │   └── StringSet.java
             └── Main.java
```

## What This Project Demonstrates

* Creating Java domain classes
* Working with Java Sets
* Managing unique objects with `HashSet`
* Sorting unique values with `TreeSet`
* Implementing mathematical set algorithms
* Modeling fixed values with enums
* Using object equality rules for collection behavior
* Processing text with regex
* Extracting and sorting unique words
* Structuring pure Java collection logic

## Getting Started

### Prerequisites

Make sure you have the following installed:

* Java 17+
* Maven
* IntelliJ IDEA or another Java IDE

### Installation

Clone the repository:

```bash
git clone https://github.com/emreyildirim-33/java-collections-set-architecture-challenges.git
cd java-collections-set-architecture-challenges
```

Run the project from your IDE or with Maven:

```bash
mvn test
```

## Notes

This project focuses on Java Collections, Set-based algorithms, enum modeling, object uniqueness, and regex-based string manipulation.

The main purpose is to demonstrate pure Java collection handling and data-processing logic through task management and text-analysis scenarios.

## Repository

GitHub: https://github.com/emreyildirim-33/java-collections-set-architecture-challenges
