# guessing.md 

``` mermaid
flowchart TD
    A([Main]) -->B[[Integer Secret]]
    B[[Integer Secret]]-->C[[Integer Guess]]
    C[[Integer Guess]]-->D(Secret=Random 20+1)
    D(Secret=Random 20+1)-->E[/Output"Please enter a guess between 1 and 20/]
    E[/Output"Please enter a guess between 1 and 20/]-->F[/Input Guess/]
    F[/Input Guess/]-->G{Guess>Secret}
    G{Guess>Secret}--True--> H[/Output Guess is too high/]
     G{Guess>secret}--False-->I{Guess < secret}
    H[/Output Guess is too high/]-->I{Guess < Secret}
    I{Guess < Secret}--True-->J[/ Output guess is too LOW/]
    I{Guess < Secret}--False-->K{{Guess!=Secret}}
    K{{Guess!=Secret}}--True--> E[/Output"Please enter a guess between 1 and 20/]
    K{{Guess!=Secret}}--False-->L[/Output Correct/]
     L[/Output Correct/]-->M([end])


```
# How I created a guessing game using Flowgorithm

1.Clicked on the down arrow  
2.Press box that says declare then double clicked it  
3.Typed "secret",clicked on the "integer" icon and then pressed "OK".  
4.Created another declare box named guess and clicked on "integer" again  
5.Clicked on the arrow beneath that box one and created an assigned box double clicked then put “secret” in variables and  “random (20) +1” in expression.  
6.Click the arrow beneath that box and selected output, enetred “please enter a guess between one and 20”.  
7.Selected arrow beneath the output box and created a "Do". _(This was where I messed up the first time as I used a "While" box, and my game started glitching out.)_but I double clicked that box and typed "guess!=secret"   
8.Selected the arrow, going to the right and created an input box called "input guess" beneath that I created an "If" box called "guess>secret" 
9.To the right of the arrow that says "True" I create an output box called  “guess is too high  
10.Then I created another "If" box and named it "guess<secret"  
11.Then to the right where it says true, I created an output box that says “guess is too low”.  
12.Then, in the "Do" box I created before I created another "Output" box name, “Correct” and pressed play. 

