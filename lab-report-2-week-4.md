![image](firstCommit.jpg)
[failure inducing code](https://asmarking.github.io/markdown-parse/test2-file.md)

bug - code did not check for when indexOf returns -1.   
Symptom - infinite loop   
Solve - if indexOf returns -1 for one of the following
']','[','(',')' then just return toReturn because there are no more links. 

![image](commitTwo.jpg)
[failure inducing code](https://asmarking.github.io/markdown-parse/test-file5.md)
bug - code did not check if the parentheses for the link came directly after the bracket ']'  
symptom - printing link "somepage.com" when it should not print anything
Solve - if the '(' does not come directly after [ then returnToreturn because it is not a link

in just 2 commits my code passed all of the Junit test on the test files provided by professor and the test files my group made