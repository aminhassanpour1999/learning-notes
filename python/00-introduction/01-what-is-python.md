# What Is Python

## Learning Objectives

By the end of this lesson, you should be able to:

- Explain what a programming language is and where Python fits.
- Describe Python's design philosophy and why readability matters.
- Summarize Python's origins and the difference between Python 2 and Python 3.
- Explain Python's main strengths: readability, ecosystem, portability, and productivity.
- Recognize important trade-offs and limitations.
- Distinguish learning Python syntax from learning to solve problems with code.

## 1. What Is a Programming Language?

A **programming language** is a formal way to express instructions that a computer can execute. It gives us rules and building blocks for describing operations, decisions, repetition, and the handling of data.

**Python** is a high-level, general-purpose programming language.

- **High-level** means that Python provides abstractions that let us express ideas without managing every low-level detail of the computer. Its syntax is designed to be comparatively readable.
- **General-purpose** means that Python is not limited to one specific type of task. It can be used in many areas, from small scripts to scientific computing and web services.

For example:

```python
print("Hello, world!")
```

This is a small Python program. It asks Python to display the text `Hello, world!`.

Python code is written by people, then executed by a Python implementation. We will explore how execution works in the dedicated lesson **How Python Runs** rather than covering those mechanics here.

An algorithm is a step-by-step method for solving a problem; a program expresses a solution in a programming language. We will study that distinction more fully in **Programming Fundamentals**.

## 2. Python's Design Philosophy and Readability

Python emphasizes readable code, clear expression, and a practical balance between simplicity and capability. Indentation is meaningful in Python: it helps show the structure of a program.

Compare these examples:

```python
total_price = 24
number_of_items = 3
price_per_item = total_price / number_of_items
print(price_per_item)
```

and:

```python
x = 24
y = 3
z = x / y
print(z)
```

Both snippets calculate the same result, but the first gives a reader more information about what the values represent. Descriptive names make code easier to understand, review, and maintain.

Readability is not just about making code look nice. It helps people find mistakes, explain their reasoning, collaborate with others, and return to their own work later. Readable code still needs to be correct, tested, and appropriately designed.

Python's design philosophy is often summarized by **The Zen of Python**. You can display it in a Python interpreter by running:

```python
import this
```

Some of its well-known principles favor readability, simplicity, and explicitness. These are guiding ideas, not a guarantee that every Python program is automatically simple or well written.

## 3. A Brief History: Python 2 and Python 3

Python was created by **Guido van Rossum**. Work on it began in the late 1980s, and it was first publicly released in 1991.

Two major versions are especially important historically:

- **Python 2.0** was released in 2000.
- **Python 3.0** was released in 2008 and introduced changes that could make some Python 2 programs incompatible without modification.
- **Python 2 reached end of life on January 1, 2020.** It no longer receives official Python 2 security updates or bug fixes from the Python project.

A couple of simple examples illustrate differences:

In Python 2, `print` was commonly used as a statement:

```python
print "Hello"
```

In Python 3, `print()` is a function call:

```python
print("Hello")
```

Division also differs in an important case. In Python 3:

```python
print(5 / 2)
```

Output:

```text
2.5
```

Python 3's `/` operator performs true division, including when both operands are integers. Python 2 had different default behavior for integer division in that case.

**For new learning and new projects, use a supported Python 3 release.** Python 2 is relevant when reading legacy code, but it should not be the starting point for a new learner.

## 4. Python's Core Strengths

### Readability

Python's syntax often lets people express an idea with relatively little code. This can make examples easier to read and prototypes easier to develop. Good names, structure, and tests are still essential.

### A broad ecosystem

Python comes with a **standard library**, which provides modules for many common tasks. There is also a large collection of third-party packages for specialized needs. This ecosystem means that programmers can often build on existing, maintained tools rather than implementing everything from scratch.

A large ecosystem is useful, but it also requires judgment: check whether a package is maintained, appropriate for the task, trustworthy, and compatible with your project.

### Portability

Python is available on major operating systems, including Linux, macOS, and Windows. Much Python code can run on different systems with little or no change.

Portability is not automatic in every case. Code that relies on operating-system-specific paths, external programs, hardware, or unavailable dependencies may need adjustments.

### Productivity

Python can be effective for experimentation, automation, scripting, prototypes, and many production applications. Its readable syntax and available libraries can help developers move from an idea to a working solution efficiently.

Productivity depends on the problem and the developer's skills. A short program is not necessarily a good program, and using a library does not remove the need to understand what the code is doing.

## 5. Trade-Offs and Limitations

No programming language is best for every task. Python has trade-offs that are worth understanding.

### Execution speed

For some CPU-intensive workloads, ordinary Python code can run more slowly than code written in languages that compile to optimized native machine code. However, performance depends on the workload and implementation. Many scientific Python libraries perform computationally intensive work in optimized native code, so a Python-based solution can still be very fast.

The practical lesson is to measure performance before optimizing, then choose tools suited to the bottleneck.

### Memory use

Python's convenient, high-level objects can involve more memory overhead than lower-level representations. This may matter when working with very large datasets or strict memory limits.

### Dynamic typing

Python is dynamically typed: names are not permanently declared to hold one particular type. For example:

```python
value = 10
value = "ten"
```

This is valid Python. The name `value` refers to an integer first and a string later. Flexibility can make code concise, but unexpected type changes can also cause bugs. Clear naming, tests, and optional type annotations can help manage this risk.

### Dependencies and deployment

A project may depend on external packages, particular Python versions, environment variables, or operating-system features. Sharing or deploying it therefore requires care with dependencies and setup instructions. We will cover project setup and environments in the relevant introduction lessons.

### Choosing the right tool

The best choice depends on the requirements: performance, available libraries, deployment environment, team experience, safety constraints, and long-term maintenance. Python is powerful, but it is not automatically the best fit for every problem.

## 6. Learning Python Versus Learning to Program

Learning a language and learning to program are related, but they are not the same.

**Learning Python** includes understanding its syntax, built-in types, functions, modules, and conventions.

**Learning to program** includes identifying the actual problem, breaking it into manageable steps, choosing a suitable approach, handling unusual cases, testing results, and improving a solution.

Consider two learners:

- Learner A can read a Python program and explain what each line does.
- Learner B can do that too, and can also analyze a new problem and develop a solution from scratch.

Learner B has practiced a broader problem-solving skill. Reading code is valuable, but independent analysis and implementation require deliberate practice as well.

To build both abilities:

1. Read and explain small programs.
2. Predict their output before running them.
3. Change one part and explain how the behavior changes.
4. Solve small problems without looking at a complete solution first.
5. Test normal cases and edge cases.
6. Review mistakes and try to explain why they happened.

You do not need to master every programming concept before writing code. Learn a concept, use it in a small task, and revisit it as problems become more complex.

## Summary

- Python is a high-level, general-purpose programming language.
- Its design emphasizes readable and expressive code.
- Python 3 is the appropriate choice for new learning and projects; Python 2 is obsolete.
- Readability, its ecosystem, portability, and productivity are important strengths.
- Execution speed, memory overhead, dynamic typing, and dependency management are among its trade-offs.
- Knowing syntax is not enough: programming also involves analyzing problems, designing solutions, and testing them.

## Exercises

Try answering these without looking back at the lesson. The goal is to explain the ideas in your own words.

1. What does it mean to call Python both **high-level** and **general-purpose**?
2. Why can descriptive variable names improve code quality? Give one example.
3. Name two differences between Python 2 and Python 3 discussed in this lesson.
4. Give two strengths and two trade-offs of Python.
5. A program runs slowly on a very large calculation. Why is it better to measure the bottleneck before deciding to rewrite it in another language?
6. What is the difference between learning Python syntax and learning to program?
7. A colleague says, “Python runs on Linux and Windows, so every Python program works identically on both.” What is incomplete about this claim?

## Knowledge Check

Before moving on, make sure you can explain, without memorizing the wording:

- What Python is and what “high-level” means.
- Why readability matters beyond appearance.
- Why new projects should use Python 3 rather than Python 2.
- Why a language's strengths do not make it the best tool for every task.
- Why solving new problems is an essential part of learning programming.

## References

- [Official Python website](https://www.python.org/)
- [The Python Tutorial](https://docs.python.org/3/tutorial/)
- [The Zen of Python — PEP 20](https://peps.python.org/pep-0020/)
- [Python 2.7 documentation (historical)](https://docs.python.org/2.7/)
