### Assignment 1
due on Mon, March 11,  at 5pm

Make a web page in your repo that colors the strings blue and the arrays red

Remove pattern selection -- it is fixed in the program

No report no demo on this Assignment


### Class work #3

Copy and modify RegExp.html -- add two interesting items in the menu

Put your work in your repo.  Send me the link your page and a screenshot.

Ref:
* https://maeyler.github.io/Auto/work/RegExp.html
* https://maeyler.github.io/JS/sss/inspector.html
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions


### Class work #2
```
Modify and combine DFA & NFA for  L = (1+0)*00
Find an array of integers less than 50 accepted by each automaton
Do the same for the RegExp  e = /00$/

     let a = [] 
     for (let n=1; n<50; n++) {
          let w = n.toString(2)  // to binary
          if (accept(w)) a.push(n);
     }

Bonus: Put your work in your repo (must be different from Auto)
```

Ref:
* https://maeyler.github.io/Auto/work/NFA1.html
* https://maeyler.github.io/JS/hard/RegExp.html
* https://www.w3schools.com/jsref/jsref_obj_regexp.asp


### Class work #1

1) How are these string concepts of Sec 1.5 implemented in JavaScript?
Alphabet, empty string, length, concatenation

2) Find an accepted string and a rejected string for the FA in Problem 2.2.11

3) Here is a model for L = (1+0)*10 = { w | binary w ends with 10 } 

Modify the code and the web page for another DFA that you choose. 

Ref:
* https://maeyler.github.io/Auto/work/DFA1.html

