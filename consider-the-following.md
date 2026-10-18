# Consider the Following: APCSA Honors WikiPracticeTest
Hello! Thank you for checking out—or even better, [contributing to](https://docs.google.com/forms/d/e/1FAIpQLSenCrKOmmAFRTI8f7P5FIQw86uHck0g7JbMsTm8TpqwlMuFeQ/viewform?usp=dialog)—**Consider the Following**, a “website” made by [Benjamin Xie](mailto:bxie80@stuy.edu) to help you practice for your APCSA Honors tests.

Jump to:
* [Guidelines](#guidelines)
* [Test01-Cumulative](#test01-cumulative)
* [Quiz02-Strings](#quiz02-strings)
* [Quiz01-Summer](#quiz01-summer)

# Guidelines
[Fill out this form](https://docs.google.com/forms/d/e/1FAIpQLSenCrKOmmAFRTI8f7P5FIQw86uHck0g7JbMsTm8TpqwlMuFeQ/viewform?usp=dialog) (stuy.edu email only!) to request contributing access.

Then read [this](https://konstantinnovation.github.io/index.html#gitbranch) for how to make contributions.

Add questions using the following format:
````
Consider the following:
```java
put your code here
```

Which of the following is correct?<br>
A. blah<br>
B. blah<br>
C. blah<br.
D. blah

<details>
  <summary>Answer</summary>
  D. This is because blah blah blah. You don't need to write an explanation, but you can if you want to. The most important is having the correct answer somewhere.
</details>

###### Written by YOURNAME

---
````

The ```` ```java ```` creates a code block, and the `---` creates a horizontal line. The `<details>` hides the answer.

If you want more cool Markdown stuff, look at [GitHub’s documentation](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) or perhaps [this “cheatsheet”](https://github.com/adam-p/markdown-here/wiki/markdown-cheatsheet#code).

One last thing: **Do not include actual test content!** This is a public website and I do not want any future students being able to just memorize the answers to the assessments with this website.

# Test01-Cumulative
This section only covers new material not covered in previous assessments. Also see:
* [Quiz02-Strings](#quiz02-strings)
* [Quiz01-Summer](#quiz01-summer)

# Quiz02-Strings
Consider the following:
```java
System.out.println('A' + 'A' - 65);
```

Which of the following will be printed?<br>
A. AA65<br>
B. -63<br>
C. 65<br>
D. error

<details>
  <summary>Answer</summary>
  C. Remember chars are just ints. 'A' is 65 (you didn’t need to know that exactly but you should have been able to figure out from the other answers). 65 + 65 - 65 = 65.<br>
  <br>
  A is incorrect. Notice the single quotes. 'A' is a character, not a String.<br>
  <br>
  B is incorrect. 'A' is 65 and not 1. You should know that letters are not at the front of the ASCII table.<br>
  <br>
  D is incorrect. You can do arithmetic with chars as if they were ints (because they are).
</details>

###### Written by Benjamin Xie

---

# Quiz01-Summer
