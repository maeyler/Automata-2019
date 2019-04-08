### Class work #6

* Modify delta() for this grammar:
```
	E -> TX
	X -> ε | +TX | -TX
	T -> FY
	Y -> ε | *FY | /FY
	F -> n | (E) | i(E) 
```
* Include several test cases such as  (n-i(n+n))/i(n*n)

* Compare and contrast Recursive-descent vs PDA implementations

Ref: 
* [PDA sample](PDA1.html)
* [Left Recursion](https://www.wikiwand.com/en/Left_recursion)
* [microJ work](../microJ/)


### Assignment 2
due on Monday, April 8, before 5pm

Beste Soft'ta ilk haftanız, daha üçüncü gün size bir iş verdiler
```
- Şu aritmetik programı var ya, Hasan Bey yazmıştı...
- Expression.html mi?
- Evet, müşteri "fonksiyonlar da olsun" diyor
- Hangi fonksiyonları koyalım?
- Ne kadar çok olursa o kadar iyi
- Math içindeki bütün fonksiyonlar?
- Orada 40 tane fonksiyon var, hangi biriyle uğraşacaksın?
- getOwnPropertyNames() ile hepsini bir kalemde yaparım
- O da ne?
- Object altında güzel bir özellik...
- Elin değmişken bir de % işlemini ekler misin?
- Hiç sorun değil... 
```
* Gramere iki yeni kural eklenecek
```
   T -> F | T*F | T/F | T%F
   F -> n | (E) | (E)^n | i(E)
```
* Hasan Bey işten ayrılmadan önce [çalışan bir jar](../microJ/exprV2.3.jar) bırakmış ama kaynak kodunu saklamış

* Math içindeki tek parametreli fonksiyonları bulmak için
```
   F = Object.getOwnPropertyNames(Math)
   a = F.filter(k => Math[k].length == 1)
```
**ÖDEVİNİZİ GÖSTERMEDEN ÖNCE REPOYA KOYMAYIN**


### Class work #5
Modify Expression.html 

1. Implement toTree() methods

2. Add one more rule for power operation
```
   F → n | (E) | (E)^n
```
Ref:
* [MicroJ Specs](../microJ/MicroJ%20Specs) 
* [Expression parser](../microJ/Expression.html) 
* [Syntax Diagram](https://www.wikiwand.com/en/Syntax_diagram) 
* [Recursive-descent Parser](https://www.wikiwand.com/en/Recursive_descent_parser) 


### Midterm
* [Question 1](../exam/midterm-1.jpg)
* [Question 2-3](../exam/midterm-2.jpg)
* [Question 4](../exam/midterm-3.jpg)

### Class work #4 
``` 
1. Study Expression.html and show a sample derivation with these rules: 
   E → T | E+T | E-T
   T → F | T*F | T/F
   F → n | (E) 
(use exactly 4 operations) 
 
2. Suggest two extensions for the grammar defined above 
 
3. Modify CFG1.html for the grammar shown below: 
S → 0S0 | 1S1 | p 
(palindromes with the mid-point mark) 
``` 
Ref: 
* [Expression parser](../microJ/Expression.html) 
* [CFG sample](CFG1.html) 
* [Quiz solution](../exam/Quiz%20solution.jpg) 
* [MicroJ Specs](../microJ/MicroJ%20Specs) 


### Quiz week

* [Lexical Analysis](https://www.wikiwand.com/en/Lexical_analysis)
* [Lexical.html](../microJ/Lexical.html)
* [MicroJ Specs](../microJ/MicroJ%20Specs.png)


### Assignment 1
due on Monday, March 11, at 5pm

Make a web page in your repo that colors the strings blue and the arrays red

Remove pattern selection -- it is fixed in the program

No report no demo on this Assignment


### Class work #3
```
Copy and modify RegExp.html -- add two interesting items in the menu

Put your work in your repo.  Send me the link your page and a screenshot.
```
Ref:
* [RegExp.html](RegExp.html)
* [Inspector](https://maeyler.github.io/JS/sss/inspector.html)
* [RegExp in Mozilla](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions)


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
* [NFA1.html](NFA1.html)
* [RegExp.html](RegExp.html)
* [RegExp in W3S](https://www.w3schools.com/jsref/jsref_obj_regexp.asp)


### Class work #1
```
1) How are these string concepts of Sec 1.5 implemented in JavaScript?
Alphabet, empty string, length, concatenation

2) Find an accepted string and a rejected string for the FA in Problem 2.2.11

3) Here is a model for L = (1+0)*10 = { w | binary w ends with 10 } 

Modify the code and the web page for another DFA that you choose. 
```
Ref:
* [DFA1.html](DFA1.html)

