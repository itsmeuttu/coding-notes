# Questions with parts and subparts (and sub sub parts)

If you want a question to have several parts, then you use the parts environment. For
example, if you type

```latex
\begin{questions}
\question
Why is there air?
\question
What if there were no air?
\begin{parts}
\part
Describe the effect on the balloon industry.
\part
Describe the effect on the aircraft industry.
\end{parts}
\question
\begin{parts}
\part
Define the universe. Give three examples.
\part
If the universe were to end, how would you know?
\end{parts}
\end{questions}
```

### Output

[https://www.notion.so](https://www.notion.so)

There is also a subparts environment, and even a subsubparts environment, and they
work just as you would expect. For example, if you type

```latex
\begin{questions}
\question
\begin{parts}
\part
What do you do with a drunken sailor?
\part
Is your answer different if it is before noon?
\end{parts}
\question
This is the second question.
\begin{parts}
\part
This is a part.
\part
This is also a part.
\begin{subparts}
\subpart
This is a subpart.
\subpart
This is a periscope.
\subpart
This is a pair of diving planes.
\subpart
\begin{subsubparts}
\subsubpart
This is a subsubpart.
\subsubpart
The lower surface of a diving plane?
\subsubpart
The ocean floor, perhaps?
\end{subsubparts}
\end{subparts}
\part
It’s sad to be apart.
\end{parts}
\question
\begin{parts}
\part
\begin{subparts}
\subpart
This is a subpart.
\subpart
This is another subpart.
\end{subparts}
\part
This is another part.
\end{parts}
\end{questions}
```

### Output

[https://www.notion.so](https://www.notion.so)