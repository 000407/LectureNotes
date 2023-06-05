# Unit 1 - Programming 

[Home](README.md) | [Prev](09_Algorithms.md)

## 10.1 Application Development 101

- Any application at a high level has the following
  - Input/Output (I/O) operations
    - storage (HDD, SSD, optical disks, magnetic disks and tapes etc)
    - telecommunication devices (NICs)
    - keyboard
    - mouse
    - microphone
    - camera
    - fingerprint scanner
    - visual display units
    - sockets and pipes
  - Processing
- Idea is to write the program using these components, to achieve the requirements.
- [Software Development Lifecycle](https://www.tutorialspoint.com/sdlc/sdlc_overview.htm)

## 10.2 Example

- A complete example of an application, developed step by step, is available [in this document](990_AppDemo.md).

## 10.3 Application Development Best Practices

### Readability & Understandability

Try to always write code that can be easily understood by others. Writing highly optimized mathematical routines, or creating complex libraries, is relatively easy. Writing 200 lines of code that can be instantly understood by another software engineer is more of a challenge.

It may seem like extra effort at the time, but this additional work will pay dividends in the future. It will make everyone's lives (including the original developer's) so much easier when returning to update the code. In addition, the debugging process should be much smoother for yourself, or for other engineers who need to edit your work.

Professionally written code is clean and modular. It is easily readable, as well as logically structured into modules and functions. Using modules makes the code more efficient, reusable, and organized.

Always remember, future-proofing the code in this way should always be prioritized over finishing quickly. It is easy to think time is saved by hacking away, but in fact, hours of extra work is being created down the line (known as technical debt).

### Ensure Code Works Efficiently

In order to optimize the code, you need to make sure it executes the function quickly. In the world of software engineering, writing code quickly and correctly is pointless if the end product is slow and unstable. This is especially true in large, complex programs. Even the smallest amount of lag can add up considerably, rendering the final application - and all of the engineering work - useless.

Equally important is minimizing the memory footprint of the code. In terms of performance, working with many functions on a large amount of data can drastically reduce the efficiency of the code.

### Refactor

Refactoring is basically improving the structure of the code, without making modifications to its actual functionality. If there are multiple blocks of code that do similar things, it is useful to refactor them into a single function. This will allow simplifying the code. Should it ever need to change how that function works, it only need to update one function rather than several.

In order to create a high-quality program, devoting time to refactor the code is essential. In the long run, refactoring will speed up the development time, and make the software engineering process much smoother.

### Professional Coding Style

A professional coding approach is not an exact science. It is a mindset that can only be developed over time, by reading and writing a lot of code, and developing the software engineering knowledge. Expert coders do not turn out unstructured blocks of code just so they can get it done quickly. Instead, their code is almost universally understandable by other engineers, no matter how much time it takes to write it.

There are a number of principles that will assist in developing an effective coding style. Some of them are:

 - Using descriptive names for functions and variables
 - Implementing modularity in the code
 - Avoiding excessive indentation

Therefore, whether the code is general (for all programming and markup languages) or production quality (specific to a particular language), it should always follow good coding convention.

### Use of Version Control

Version control refers to a software engineering framework that tracks all changes and synchronizes them with a master file stored on a remote server. An effective version control system is a key aspect of writing production code. Using version control in a professional project will enable the following benefits:

 - In case the system crashes, the entire code is backed up on the server.
 - All members of the software engineering team can sync their changes regularly by downloading them from the server.
 - Numerous developers can work independently to add/remove features or make changes to a single project, without impacting other member’s work.
 - If serious bugs are created, it is always possible to return to a previous, stable version of the codebase that was known to work.

### Developer Testing

Good testing practices not only ensure quality standards in software engineering, but also guide and shape the development process itself. Testing ensures the code gives the desired result and meets all necessary user requirements.

Unit tests are used to test small, self-contained parts of the code logic. These engineering tests are designed to cover all possible conditions. The process of writing the test is beneficial in itself. It requires figuring out the behavior of the code and how it will be tested. Small and regular tests are better than one large test after completion. This approach helps maintain a modular structure and will result in a higher quality end product.

### Keep It Simple, Stupid

The popular acronym ***KISS***, noted by the U.S. Navy in 1960, is extremely relevant in the software engineering community. It stands for &quot;Keep It Simple, Silly&quot; (some variations replace &quot;Silly&quot; with &quot;Stupid,&quot;). Whatever the variations, the underlying idea remains the same.

The keyword here is &quot;Simple,&quot; and the idea is to keep the code as concise as possible. In the context of coding, this means making the code meaningful, to-the-point, and avoiding unnecessary engineering work.

The KISS Principle ensures that the code has high maintainability. You should be able to go back and debug it easily, without wasting time and effort.

###  YAGNI - You Ain't Gonna Need It

Another acronym that’s popular among software engineers, YAGNI means &quot;You Aren’t Gonna Need It&quot;. This principle focuses on eliminating any unnecessary coding and works in tandem with the KISS principle.

Instinctively, meticulous engineers start by planning and listing everything that ‘might be used’ during the project. However, sometimes they end up with components that are never used.

So it’s always a good idea to avoid coding something that you do not need &quot;right now.&quot; You can always add it later if circumstances change.

### DRY - Do not Repeat Yourself

Like the previous two points, the DRY (Don’t Repeat Yourself) Principle aims at reducing repetition and redundancies within the software engineering process. This is achieved by replacing repetitions with abstractions or by grouping code into functions.

If the code is performing the same instruction in 6 different places, it can be a real struggle to manage, even for experienced engineers. Let us say it is decided to change how that instruction works. It will be required to update the code 6 times for just 1 change. It is therefore much better practice to create a single function that performs the instruction once, and reference this function each time it’s needed. If it requires to change how it works, there will be only one update.

## General Tips

Some tips and techniques can be applied to any coding language and are useful in improving the overall quality of the code:

 - Allocate appropriate names to all functions, variables, and methods. This will make the code easier to read, understand, and debug.
 - Always use the common or native language of the developer for names and descriptive texts. Avoid abbreviations as much as possible to reduce ambiguity.
 - Use consistent indentation and alignment while formatting the code for better readability.

***
[Home](README.md) | [Prev](09_Algorithms.md)