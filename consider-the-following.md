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
C. blah<br>
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

Consider the following:

i.
```java
String[] arr = new String[5];
for (int i = 0; i < arr.length; i++){
  System.out.println(arr[i]);
}
```

ii.
```java
int count = 0;
String[] arr = new String[5];
for (int i = 0; i < arr.length; i++){
  if (arr[i].equals("hi")) count++;
}
System.out.println(count);
```

iii.
```java
int[][] arr = new int[3][2];
for (int i = 0; i < 3; i++){
  System.out.println(arr[0][i] != arr[1][i]);
}
```

Which of the above will result in a `NullPointerException`?<br>
A. i only<br>
B. iii only<br>
C. i and iii only<br>
D. i, ii, and iii<br>
E. none of these options

<details>
  <summary>Answer</summary>
  E is the correct answer.<br>
  <br>
  i. Creates a new String array—by default each of the items are null. When you print something that is null, you will get "null". Not a NullPointerException.<br>
  <br>
  ii. Creates a new String array—by default each of the items are null. Even though this is a String array, you can’t use .equals or other methods on null. If you try to, you will get a NullPointerException.<br>
  <br>
  iii. Creates a new 2D int array with 3 rows and 2 columns. Each element is by default 0, not null, so automatically this should not be a NullPointerException. This actually still breaks, but for a different reason (ArrayIndexOutOfBoundsException).<br>
  <br>
  The option we want, ii only, is not present, so we should choose E. none of these options.
</details>

###### Written by Benjamin Xie

---

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

Consider the following:
```java
String str = new String "Hello\nWorld\"";
System.out.println("Goodbye " + str.substring(5));
```
Which of the following will be printed?<br>
A. Goodbye \nWorld"<br>
B. Goodbye <br>  World"<br>
C. Goodbye World<br>
D. error

<details>
  <summary>Answer</summary>
  B. \n is the character at index 5; escape sequences like \n are regarded as a single character. \n creates a new line, meaning there is a break between "Goodbye" and "World".<br>
  <br>
  A is incorrect. \n is an escape sequence, so it would start a new line instead of printing "\n".<br>
  <br>
  C is incorrect. \n is an escape sequence, so it would start a new line. str.substring(5) includes the character at index 5 up to the last character. <br>
  <br>
  D is incorrect. Both escape sequences are valid; if they were invalid (ex. \!) it would return an error. In this case, it doesn't.
</details>

---

# Quiz01-Summer

