# guessing.md
guessing game 

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
