# **Bug Diff**

I used the `diff` command in order to find deltas between my own implementation and the one provided.

![command](vimdiff.png)

## *First Difference Found*

[139.md](https://github.com/nidhidhamnani/markdown-parser/blob/8dd87e6914ae40a4321aac8e2483e349de40b03c/test-files/139.md) is the file that causes this issue.

The first difference I found was when the implementation we were given gave an empty ArrayList. This was incorrect since there was no empty link given in the test files. The implementation written by me did not return anything, which was what was expected. 
![diff1](diff1.png)
![raw1](raw1.png)

The issue with the code is that it checks for links within code blocks but does not stop producing and instead returns an empty ArrayList instead of nothing when a link is not found. This is where a fix needs to be produced in the code:
![fix1](fix1.png)

## *Second Difference*

[341.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/341.md) is the file that causes the difference.

![diff2](diff2.png)
![raw2](raw2.png)

According to the `.md` file linked above, there should have been nothing returned. However, the implmentation fails to account for the fact that other characters such as the asterisk and when looking for code blocks the program uses the text as a link and formats as if there is still text.

![fix2](fix2.png)

The program should have taken into account the initial difference in code blocks without links and also should therefore check for other characters that overlap with the code block sequences as well as title or link sequences.