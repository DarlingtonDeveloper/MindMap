---
title: C# Quiz Topic Breakdown
description: A structured breakdown of key C# topics based on a high-difficulty assessment, formatted for Quartz
---

# C# High-Level Assessment Topics

This page outlines the major topics covered in an advanced-level C# test, organized to help you review or create educational content. Each section represents a key area tested in the exam.

---

## 🧵 Threading & Concurrency
- `Interlocked.Increment`
- `Monitor.Enter` / `Monitor.Exit`
- Thread-safe access to shared data
- `Task` vs `Thread`
- Task status and lifecycle (`Status`, `IsCompleted`, `Faulted`)
- Thread construction, data passing
- Thread start limitations

## 🧪 Pattern Matching
- `is` pattern with `switch`
- List patterns (`[1, 2, ..]`, `[.., >5]`, etc.)
- Positional and property pattern matching
- `when` guards

## 🧰 Reflection & Metadata
- Accessing custom attributes like `[Serializable]`
- `AssemblyVersionAttribute`
- Reflection APIs (`GetType()`, `GetCustomAttributes()`)
- Using `dynamic` with `Activator.CreateInstance`
- Loading assemblies via `Assembly.LoadFile`

## 🔠 Regular Expressions
- Matching US phone numbers
- Anchors (`^`, `$`)
- Quantifiers (`{3}`, `*`, `+`, `?`)
- Special characters (literal vs control)
- Splitting camel case strings

## 🔧 File I/O & Streams
- `MemoryStream` and its behavior
- `File.WriteAllText`, `FileStream`
- `Seek()` vs `Position`
- Overwriting vs appending files
- Directory operations and locking

## ⚡ Events & Delegates
- Declaring and invoking `EventHandler`
- Null-safe invocation using `?.Invoke()`
- Thread-safe event raising
- Multicast delegate behavior
- Event subscription duplication

## 🧮 Math & Generic Constraints
- `INumber<T>` (C# 11+ / .NET 7+)
- Generic math in .NET
- `where T : notnull, INumber<T>`
- Type safety in generic methods
- Null handling in generics

## 🔐 Security Algorithms
- AES, RSA: secure algorithms
- DES, 3DES: deprecated algorithms
- SHA: hashing, not encryption

## 🔤 String & Regex Methods
- `Replace`, `ToUpper`, `Normalize`
- Regex for pattern validation

## 🧱 Structs vs Records
- Use cases
- Value vs reference semantics
- Equality behavior
- Inheritance restrictions
- Record struct mutation (`with`, init-only props)
- Overriding `ToString` in structs

## ⚙️ Module Initializers
- `ModuleInitializer` attribute (C# 9+)
- Constraints (must be static, parameterless, non-generic)

## 🧩 Dynamic Typing
- `dynamic` vs `var`
- Runtime binding and DLR
- Limitations and performance

## 🧾 Assembly & Imports
- `using` vs `global using`
- File-scoped types (`file class` in C# 11)
- Accessibility of file-level types

## 🔐 Access Modifiers and Property Accessors
- `init` keyword
- `private set`, `private get`
- Constructor behavior with accessors

## 🧭 Performance Monitoring and Debugging
- `PerformanceCounter`
- Conditional breakpoints
- `Debugger.Break()`
- Evaluating system metrics

## 🎭 Reference Types and Ternary Operators
- `ref` keyword
- Conditional expressions with `ref`
- Referencing array elements conditionally

## 🌐 Implementing IEnumerable
- `yield return`
- Interface implementation
- Iterator patterns

---

## 📌 Tip:
You can use this structure to create individual Markdown pages or flashcards for focused study or learning resources.
