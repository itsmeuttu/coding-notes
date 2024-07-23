# Asking Questions

Once you’ve typed **\begin{document}** and (if the students will be writing their answers on
the question pages) asked for the student’s name , you can list the questions
on the exam in a questions environment. You begin each question with a **\question**
command, which is optionally followed by a number of points inside of square brackets. For
example, if you type

```latex
\begin{questions}
\question[10]
What is chemical formula of water?
\question[15]
How much wood would a woodchuck chuck if a woodchuck could chuck
wood?
\question[10] Compute $\displaystyle\int_0^1 x^2 \, dx$.
\end{questions}
```

### Output

![Untitled](Asking%20Questions%2064fde0b54a7843fc95a35e48efaa93b8/Untitled.png)