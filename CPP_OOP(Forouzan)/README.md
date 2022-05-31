Book goes into decent detail visually with code examples regarding some of the primitive language functionalities such as types, loops, conditionals, functions, et cetera. However like all things read, some skepticism is healthy.

Section 7.2.4 which goes into function inlining incorrectly states that if the body of a function is "short" (whatever that means, a metric or quantification was not defined for what is determined to be "short") then the body of the function will be inherently inlined. While this is somewhat true, it's also not.

Functions can be inherently inlined if their body evaluations and expressions are non complex, and has nothing to do with the length of the body. This section also felt a bit misplaced being in the middle of the section going over classes.

The subsection on constructors details the constructor and destructor being two special member functions but does not explain that there are two others (if using C++03 or earlier) or 4 others (if using C++11 or later), however briefly goes into copy constructors.

This section also skips out on explicit/restricted constructors, as well as move semantics. However this is a beginner targetted book so I'm not sure if those subjects would be more confusing than informative.

The book also does not explain that static data members' lifetime starts at program execution and ends when the program ends. Merely, somewhat about what a static data member is and how to declare one is defined, rather than when to and when not to use them.

A section of Object Oriented programming starts at about 1/3rd of the way through the book in section 7.6 and doesn't really do a justice to its-self for a book apparently focused on OOP (C++ Programming *An Object Oriented Approach*). This pidly little section goes into more detail about 3 types of files (Interface, Implementation, Application) and barely at all into encapsulation, before moving onto arrays. Very disappointing.

The arrays section is pretty good, it goes into how indexing works, construction of an array, the subscript operator, out of range errors, multidimensional arrays, etc. This section has some pretty good visual material to help the reader.

Chapter 9 which goes into references, pointers, and memory management. It gives an example in which a reference cannot bind to an rvalue, however it doesn't really explain that there's another type of reference called an rvalue reference which can. However going into rvalue refs can also lead into xvalues and prvalues, which may be out of scope for beginners.

The end of the references section of chapter 9 goes into when to use pass by reference vs pass by value, and states that if you ever need to change something, you should use pass by ref. While this is sometimes the case, sometimes it's also not. Primitive values can be passed by value and changed through a return statement, and some compilers (C++11 and higher) may perform extra work to create a reference, however if you're using a compiler running C++03, just use pass by ref.

The section on pointers could do a bit more effort at explaining what pointers are and what they're used for. The introductory paragraph states "A pointer variable is a variable whose contents are of pointer type." A beginner is going to read that and most likely ask "Okay but I'm still confused about what a pointer is." It's like that whole "In order to understand recursion, you must first understand recursion" joke.

The pointer arithmetic section is always going to be confusing to those who're new to pointers, let alone evaluating mathematics with them. The visual ques are decent, but this topic will almost always require further research beyond a book explaining some of it. Although it does an okayish job at it.

The inheritance section does not go into virtual inheritance (or "diamond inheritence") to address the issue of each derived class creating its own instance of a base class. It's not until the next chapter which goes into polymorphism that the problem is addressed later into the chapter. So a bit of inconsistency regarding the order at which topics are discussed.

Smart pointers are covered in the chapter after polymorphism which is operator overloading, which I feel is incorrect. Smart pointers in my opinion should either be covered in a chapter on Standard Template Library improvements or should be covered alltogether along with the new/delete operator in the previous pointers chapter.

The exceptions section is fine for the most part, however does not explain that exceptions are heavy and can be costly, or how most functions inherently come with a noexcept specifier and that explicitly including it in your function declaration can sometimes improve efficiency.

The templates section does a fine job of giving an overall general idea behind templates and their implementation (although unfortunately avoiding variadic templates), however templates being such a deep and wide topic deserves its own book entirely (Which I have and will be writing a review for as well).

[To Be Added] The Data Structures and Algorithms section will be added/reviewed at a later date.

The STL section does a great job of covering quite a bit of the STL. I'd argue much more than learncpp did which was great.

Overall, it's a pretty good book, I bought the paperback version which is for students outside of the US; which at the time is worth $63, whereas the Hardcover US version is $50 rent, about $100 used. Much of what I learned on learncpp is covered in the book, although learncpp is free, the book does include many visually assisting explanations/diagrams to help people who may have a harder time understanding something.
