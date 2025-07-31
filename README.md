🗃️ Arrays and Strings in C++
🎯 AIM

To understand and implement arrays and strings in C++, exploring their characteristics, operations, and common algorithms for efficient data manipulation.
📚 THEORY
📌 Arrays

An array is a collection of elements of the same data type stored contiguously in memory. It allows multiple values under a single variable name, accessible by zero-based indices.

    Fixed size known at compile time
    Homogeneous data type
    Efficient indexed access

📌 Strings

A string is a sequence of characters terminated by a null character ('\0'). C++ supports:

    C-style strings: Character arrays ending with '\0'
    std::string class: Safer, flexible string handling from the Standard Library

🔄 Common Operations
Operation 	Arrays 	Strings
Traversal 	Using loops (for, while) 	Using loops or string methods
Search 	Linear or binary search algorithms 	find(), find_first_of() etc.
Modification 	Element assignment by index 	Modify characters or use string methods
Concatenation 	Manual element copying 	strcat() (C strings), + or append()
Sorting 	Standard algorithms like sort() 	Sorting characters or string arrays
⚙️ Best Practices and Optimization Tips

    ✅ Always ensure array bounds are respected to avoid undefined behavior.
    ✅ Prefer std::string over C-style strings for safety and convenience.
    ✅ Minimize copying large arrays or strings; use references or pointers where applicable.
    ✅ Use standard library algorithms (<algorithm>) for sorting and searching to leverage optimized implementations.
    ✅ For large datasets, consider dynamic arrays (std::vector) instead of fixed-size arrays.

📋 Algorithm
✅ Calculate Sum and Average of Marks

    Start
    Declare an integer n = 6
    Declare and initialize an array:
    marks[n] = {100, 200, 300, 400, 500, 600}
    Set key = 400 to search
    Initialize sum = 0, avg
    Loop i from 0 to n-1:
        If marks[i] == key, print index and break
    Loop j from 0 to n-1:
        Add marks[j] to sum
    Calculate average as avg = sum / n
    Display sum and avg
    End

✅ Find Maximum in an Array

    Start
    Input an array arr[] and size n
    Initialize max = arr[0]
    Loop from i = 1 to n-1:
        If arr[i] > max, set max = arr[i]
    Print the maximum value
    End

✅ Reverse a String (Without Using reverse() Function)

    Start
    Declare strings: str1, str2
    Input string into str1
    Calculate length n = str1.length()
    Loop i from n - 1 to 0:
        Print str1[i]
    End

✅ Check if a String is a Palindrome

    Start
    Declare a for input, revstr for reversed string
    Input string into a
    Get length using a.length()
    Loop from i = length - 1 to 0:
        Append a[i] to revstr
    Compare a and revstr:
        If equal → Print "It is a palindrome"
        Else → Print "It is not a palindrome"
    End

🧠 CONCLUSION
Arrays and strings are fundamental data structures in C++ programming. Understanding their properties and mastering operations such as traversal, searching, modification, and concatenation enables programmers to manipulate data efficiently. Using loops and standard algorithms helps in solving complex problems, such as calculating averages, finding maximum values, reversing strings, and checking palindromes. Adhering to best practices like boundary checking, preferring std::string over C-style strings, and leveraging the Standard Template Library ensures safe, clean, and optimized code. Mastery of arrays and strings forms a strong foundation for advanced programming concepts and real-world applications.
