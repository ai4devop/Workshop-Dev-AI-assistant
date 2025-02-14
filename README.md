# WORKSHOP AI4GEN : Dev AI assistant
Welcome to this training based on teaching you the different possibilities of AI assistant, it will show you how your AI can assist you in you daily life as a coder.
<br>
You will see differents use cases where it can be useful
<br>
Ready ? Let's go
<br><br>

## Prerequisites
- AI assistant installed and ready on your IDE <br>
Warning : If another AI tool is installed on your IDE, it might block some of the shortcut/options, if so, you can disabled for the moment the other tools to work with this training
<br><br>

## AI assistant

### New Project
Create a new project on your IDE for this training<br>Ask on your AI chat to generate a new project in the programming language you want<br>Then add the said code in a new file.
<details>
    <summary>Click to reveal the solution</summary>

    Generate a project in [Your-programming-language]

</details>

Note : you can remove the default "hello world" code that have been generated
<br><br>

 ### Code generator
 1) In the main of your project, ask your AI to create two variables (iInput1 and iInput2) that will ask user to make integers inputs
 <details>
    <summary>Click to reveal the solution</summary>

    Write in [Your-programming-language] a code that take two integers from the user and put it in iInput1 and iInput2

</details>
<br><br>

2) Run a new AI chat and copy paste this text in french to your chat<br>(in the text, switch the brackets [your-programming-language] by the language you use)<br>Add your AI's result to your code (we will see later what the code do)
<details>
    <summary>French text to copy paste</summary>
    Créer une fonction en [your-programming-language] qui se nommera "etrangeFonction" qui va faire le calcul du plus grand diviseur commun entre deux variables données en paramètre et retournera la valeur. Dans cette fonction n'écrit aucun commentaire, n'utilise que des noms de variable abstrait. Je veux seulement cette fonction et pas d'autre code autour
</details>
<br><br>

3) Now, use AI to change the code in python that I will give you to a code in your programming language<br>Add your AI's result to your code
```python
def secondFonction(a, b):
    iCalcul = etrangeFonction(a, b) - 1
    return (10 / iCalcul)
```
Note : If you're using python as your programming language, change the given code to another language that you know, the goal here is to show you that AI can understand your code and modify it to another language
<details>
    <summary>Click to reveal the solution</summary>

    Rewrite this code from python to [your-programming language] :
    def secondFonction(a, b):
        iCalcul = etrangeFonction(a, b) - 1
        return (10 / iCalcul)
</details>
<br><br>

4) Write a prompt to use the secondFonction with the parameters iInput1 and iInput2
<details>
    <summary>Click to reveal the solution</summary>
    Call the function secondFonction with iInput1 and iInput2
</details>
<br><br>

5) Run the code given and test this values<br>input1 = 22<br>input2 = 33<br>Should give you as result = 1
<br><br>
input1 = 5<br>input2 = 6<br>Should give you as result = error division by 0
<br><br>
If it is not the result that you have, call the admin
<br><br>




### Maintenability
1) Hmm... Strange, why do we have an error with that test ?<br>It must be the function "etrangeFonction" that I gave you but.... What does it do ?<br>Let's see (assuming you don't know what this function does)<br><br>Select the whole function "etrangeFonction"<br>And copy paste it in a new AI chat<br>Ask your AI, what does this code do<br>So, what does that code do ?
<details>
    <summary>Click to reveal the solution</summary>
    The function "etrangeFonction" calculates the greatest common dividor (GCD) of two numbers
</details>
<br><br>

2) Seems like this code is good and quite simple, so it is the secondFonction that have an issue making this division by 0. We should have add some protection around this<br><br>Select the whole function "secondFunction"<br>And copy paste it in the AI chat<br>Then ask your AI to fix it
<details>
    <summary>Click to reveal the solution</summary>
    Can you fix this code ?
    Add protection to this code to check the denominator
</details>
<br><br>

3) Now it should be better.... But with that much modification, we have a big spaghetti code, maybe we should refactor this file<br>Take your code and add it to your AI chat and ask to refactor it<br>Note : You can do it like that because it is a small file with few code lines, if your file is much bigger or if you want to refactor only a part of your code (which is a better method to do), select only the part of code then ask to your AI<br>If the code is correct to you, you can now copy paste the generated code and replace yours
<details>
    <summary>Click to reveal the solution</summary>
    Refactor this code
</details>
<br><br>

4) We might need to test our code, that would be great<br>Select the "etrangeFonction" whole function code<br>Copy paste to your AI chat and ask to generate test<br>If the code is correct to you, you can follow your AI instructions to add tests to your file
<details>
    <summary>Click to reveal the solution</summary>
    Generate unit tests on this code
</details>
<br><br>

5) Great, this new code should be fine now, we should write documents about some parts of this code<br>Select a part of code that you want docs<br>Copy paste it to your AI chat<br>Then ask your AI to comment and write docs about it
<details>
    <summary>Click to reveal the solution</summary>
    Write comments in this code
    Write a documentation explaining what this code do
</details>
<br><br>

6) If you forgot to write docs to a function and try to re-understand what does the code do<br>Select the part function that you want to understand<br>Add it to your AI chat and ask for an explanation
<details>
    <summary>Click to reveal the solution</summary>
    Explain this code
</details>
<br><br>
