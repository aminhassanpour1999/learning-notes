# Python Documentation

## Learning Objectives

- Recognize the main parts of the official Python documentation.
- Choose the right reference for a question.
- Read examples and API descriptions carefully.
- Check which Python version a page describes.
- Use documentation together with small experiments.

## 1. Why Documentation Matters

Documentation is a primary source for learning how a language and its libraries are intended to work. It can explain syntax, behavior, function arguments, return values, exceptions, examples, and compatibility notes.

Search results, tutorials, and forum posts can be useful, but they may be outdated or omit important conditions. When a question concerns Python's actual behavior, consult the official documentation and test a small example when possible.

You do not need to read all documentation from beginning to end. Learn how to find the relevant page and extract the information needed for the current problem.

## 2. The Python Tutorial

The **Python Tutorial** is a guided introduction to Python's main language features. It is especially useful for learning the language in a structured order and seeing examples in context.

The tutorial assumes some familiarity with programming concepts, so a beginner may need additional explanations and practice. Use it as a reference and learning path, not as a replacement for solving exercises yourself.

## 3. The Language Reference

The **Language Reference** describes Python's syntax and core language semantics in more formal detail. It is useful when you need a precise answer about how a language construct is defined.

It is more technical than the tutorial. Beginners do not need to memorize it, but knowing that it exists helps when a tutorial-level explanation is insufficient.

## 4. The Standard Library Reference

The **Standard Library** documentation describes modules included with Python, such as tools for mathematics, paths, dates, JSON, CSV, testing, and file handling.

When looking up a function or module, check:

- The exact name and purpose.
- The parameters it accepts.
- The value it returns, if any.
- Exceptions it may raise.
- Important side effects or platform limitations.
- Examples and version notes.

Do not assume that every package mentioned in a tutorial is part of the standard library. Third-party packages generally have their own documentation and installation requirements.

## 5. The Glossary

The official **Glossary** defines technical terms used throughout the documentation. It can help clarify words such as *iterable*, *hashable*, *argument*, *parameter*, and *scope*.

Technical words sometimes have a more precise meaning in programming than in everyday conversation. When an explanation depends on a term, look it up rather than relying on a vague guess.

## 6. Python Packaging User Guide

The **Python Packaging User Guide** covers packaging projects, installing packages, and related tools and practices. It becomes particularly useful when moving beyond one-file programs to projects with dependencies or when sharing code with others.

Package installation commands and environment setup depend on the project and system. Follow current official guidance rather than copying commands without understanding which interpreter and environment they affect.

## 7. Version-Specific Documentation

Documentation pages usually describe a particular Python version. A feature or behavior available in a newer release may not exist in an older one, and a third-party library may support only a subset of Python versions.

When an example fails:

1. Check the Python version you are running.
2. Check the version described by the documentation.
3. Check whether the feature or argument exists in both versions.
4. Read the error message and nearby documentation.
5. Try a minimal reproducible example.

Avoid assuming that an online answer from several years ago still applies unchanged.

## 8. A Practical Documentation Workflow

When you encounter an unfamiliar function:

1. Search for the function in the official documentation.
2. Read the overview and signature.
3. Identify its inputs, output, exceptions, and side effects.
4. Study one example.
5. Run a small example locally.
6. Modify the example to test your understanding.
7. Record the rule and link in your notes if it will be useful again.

For example, if you are unsure how `round()` behaves, read its official description, try a few inputs, and compare the results with your expectation. A tiny experiment often makes a definition easier to understand.

## Summary

The official documentation includes a guided tutorial, a formal language reference, standard-library reference, glossary, and packaging guide. Choose the source that matches your question, check its version, and combine reading with small experiments.

## Exercises

1. Which documentation section would you consult for a guided overview of Python's language features?
2. Where would you look up a built-in function's parameters and return behavior?
3. Why should you check the version of Python described by a documentation page?
4. Explain the difference between the standard library and a third-party package.
5. Choose one built-in function, read its official documentation, and write down its purpose, inputs, output, and one example.
6. Find an unfamiliar technical term in the official glossary and explain it in your own words.

## Knowledge Check

You should be able to choose an appropriate official reference, extract the key details of an API, and verify your understanding with a small local example.

## References

- [Python documentation home](https://docs.python.org/3/)
- [The Python Tutorial](https://docs.python.org/3/tutorial/)
- [The Python Language Reference](https://docs.python.org/3/reference/)
- [The Python Standard Library](https://docs.python.org/3/library/)
- [The Python Glossary](https://docs.python.org/3/glossary.html)
- [Python Packaging User Guide](https://packaging.python.org/en/latest/)