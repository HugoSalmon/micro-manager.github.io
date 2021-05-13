---
autogenerated: true
title: Micro-Manager Coding Style and Conventions
layout: page
---

## Micro-Manager Coding Style

**Formatting and style**

-   All indents are 3 spaces (no tab characters).
-   Curly braces open in the same line in Java and in a new line in C++
    (see examples).
-   Class names begin with uppercase, and with each word capitalized,
    e.g. `MyFirstClass`.
-   Function names use the same convention except that in Java they
    begin with lowercase and in C++ with uppercase, e.g. `MyFunc()` in
    C++ and `myFunc()` in Java.
-   All variables begin with lower case, e.g. `myVar`.
-   Class member variables begin with lowercase and end with underscore,
    e.g. `memberVar_`.
-   Do not use `this->memberVar_` idiom unless it is absolutely
    necessary to avoid confusion.
-   Static constants in C++: `const char* const g_Keyword_Description`.
-   Static constants in Java: `static final String METADATA_FILE_NAME`.
-   `if/else`, `for`, and `while` statements should include curly
    braces, even if they are only followed by a single line.
-   For Java code, follow the [Java style recommendations at
    Geosoft](http://geosoft.no/development/javastyle.html#Recommendation).

**Comments, headers, etc…**

-   Function/class headers use documentation JavaDoc convention (see
    examples).
-   The code should be clear and self explanatory.
-   Use comments to explain algorithms and anything that is not self
    evident.
-   Function headers should explain the “contract” with the caller if it
    is not totally clear from the function signature (parameters). In
    general all public methods should have headers.
-   Use common sense and avoid unnecessary headers and comments for code
    that is obvious.
-   In general, do not enter revision history comments in the source
    code, nor in the file header. They impair readability and break the
    visual flow.

**Revision/change tracking**

-   Only the latest version matters. Keep the code elegant and simple
    (both visually and functionally).
-   Use source code control to retain the revision history in the
    particular file, i.e. check in the SVN often and each time enter the
    revision history comment.
-   Work incrementally. Make small changes and make sure the code
    compiles. Check-in after every major step to retain revision
    history.
-   If there is a danger of destabilizing the main application, open a
    branch and work in it for a while, but still check in at least once
    each day.

## Micro-Manager Coding Conventions

### Exceptions in mmstudio

`org.micromanager.utils.ReportingUtils` is a static Java class that
contains methods to simplify reporting Java errors and exceptions to the
user and logging them in the CoreLog. The class methods
`ReportingUtils.showError(...)` or `ReportingUtils.logError(...)` should
be used in catch blocks. `ReportingUtils.showError(...)` is useful for
infrequent exceptions, while `ReportingUtils.logError(...)` should be
used in loops so that the user is not force to acknowledge a whole
series of errors.

You can automate generation of such catch blocks in Eclipse by going to:

```
Preferences > Java > Code Templates > Code > Catch block body > Edit...
```

and change the Pattern to:

```
// ${todo} Auto-generated catch block
ReportingUtils.showError(${exception_var});
```

{% include Programming_Sidebar text="" %}