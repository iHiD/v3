---
name: "[C#] Add new concept exercise: <SLUG>"
about: Add the [SLUG] concept exercise to the C# track
title: "[C#] Add new concept exercise: <SLUG>"
labels: track/csharp, exercise/concept
assignees: ""
---

# C# - Add new concept exercise: <SLUG>

This issue describes how to add a new [C# concept exercise][docs-concept-exercises] named `<SLUG>`.

## Goal

A clear description of which concepts this exercise aims to teach.

For example:

The goal of this exercise is to teach the student how concept X is implemented in C#. We will teach X through C#'s Y type.

## Things to teach

A list of things the exercise aims to teach the student.

For example:

- Know of the existence of type `Y`.
- Know of some basic functions that work on `Y`.
- Know where `Y` is documented, or at least how to search for it.
- ...

## Things not to teach

A list of things that are outside the scope of this exercise and that the exercise should thus not teach.

For example:

- Memory and performance characteristics of `Y`.
- Advanced usage of `Y`.
- ...

## Resources to refer to

List suggestions to use for resources in the exercise's documentation file(s).

For example:

### Hints

- [How to use `Y` when doing `A`][http://test.com]
- ...

### After

- [Performance characteristics of using `Y`][http://test.com]
- ...

## Concepts

List the concepts this exercise teaches. These concepts can be more fine-grained than their overarching concepts.

For example:

- `basic-strings`
- ...

## Prequisites

List the prerequisite concepts that this exercise expects the student to already be familiar with.

For example:

- `basic-numbers`
- ...

## Representer

If this exercise requires any modifications to the track's representer, list these changes here and the reason for these changes.

For example:

- Normalize ternary expressions to if statements, as we are not interested in the type of conditional that is used.
- ...

To help the implementer get started, add a link to the [C# representer document][docs-representer].

## Analyzer

If this exercise requires an analyzer to be added for it, list the patterns the analyzer should detect here.

For example:

- If feature `K` is used, suggest using feature `L`.
- ...

To help the implementer get started, add a link to the [C# analyzer document][docs-analyzer].

## Implementing

If you'd like to work on implementing this exercise, the first step is to let us know through a comment on this issue, to prevent multiple people from working on the same exercise.

Implementing the exercise means creating the following files:

<pre>
languages
└── csharp
    └── concept-exercises
        └── &lt;SLUG&gt;
            ├── .docs
            |   ├── after.md (optional)
            |   ├── hints.md
            |   ├── instructions.md
            |   └── introduction.md
            ├── .meta
            |   ├── config.json
            |   └── Example.cs
            ├── &lt;NAME&gt;.cs
            ├── &lt;NAME&gt;Test.cs
            └── &lt;NAME&gt;.csproj
</pre>

- `<NAME>.cs`: the stub implementation file, which is the starting point for students to work on the exercise.
- `<NAME>Test.cs` file with the exercise's test suite.
- `<NAME>.csproj`: the C# project file.
- `.meta/Example.cs`: an example implementation that passes all the tests.
- `.meta/config.json`: the exercise's configuration file. This file specifies the solution file, test file, and should contain all tests and the methods they call.
- `.docs/introduction.md`: provides an introduction to the concept. It should be explicit about what the exercise teaches and maybe provide a brief introduction to the concepts, but not give away so much that the user doesn't have to do any work to solve the exercise.
- `.docs/instructions.md`: provides instructions for the exercise. It should explicitly explain what the user needs to do (define a function with the signature `X.y(...)` that takes an A and returns a Z), and provide at least one example usage of that function. If there are multiple tasks within the exercise, it should provide an example of each.
- `.docs/hints.md`: if the user gets stuck, we will allow them to click a button requesting a hint, which shows this file. The file should contain both general and task-specific "hints". These hints should be enough to unblock almost any user. They might link to the docs of the functions that need to be used.
- `.docs/after.md` (optional): once the user completes the exercise they will be shown this file, which gives them any bonus information or further reading about the concept taught.

## Inspiration

When implementing this exericse, it can be very useful to look at already implemented C# exercises like the [strings][exercises-concept-strings] or [dates][exercises-concept-dates] exercises. You can also check the [language-independent reference documents][general-reference] to see if there is a document for the concept(s) this exercise implements. If so, these documents have links to all language tracks that have already implemented an exercise for that concept.

## Help

If you have any questions while implementing the exercise, please post the questions as comments in this issue.

[exercises-concept-strings]: ./languages/csharp/concept-exercices/strings
[exercises-concept-dates]: ./languages/csharp/concept-exercices/dates
[docs-concept-exercises]: ./languages/csharp/docs/concept-exercises.md
[docs-analyzer]: ./languages/csharp/docs/analyzer.md
[docs-representer]: ./languages/csharp/docs/representer.md
[general-reference]: ./reference
