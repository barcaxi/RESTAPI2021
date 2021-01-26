---?color=black
@title[Title]

@snap[west headline text-white span-70]
TypeScript
@snapend

@snap[south-west]
@fa[envelope-o pad-right-icon]@css[contact-email](thomas.devine@lyit.ie)
@snapend


---
@title[Contents]
### Contents

@ol[](false)
- What is TypeScript?


@olend

---
@title[Contents]
### Contents

@ol[](false)
- **What is TypeScript?**


@olend

---
@title[What is TypeScript?]
### What is TypeScript?


![images/4_TypeScript.png](images/4_TypeScript.png)


@ul[list-bullets-black](false)
- TypeScript is a superset of JavaScript
- All TypeScript code is valid JS code...
@ulend

---
@title[What is TypeScript?]
### What is TypeScript?

@ul[list-bullets-black](true)
- TypeScript is the programming language used by **Angular**
- But TypeScript (TS) has features JS doesn't have, like...
@ulend



---
@title[What is TypeScript?]
### What is TypeScript?

TypeScript (TS) features:

@ul[list-bullets-black](true)
- Strong data typing (optional)
- OO features 
  - classes
  - interfaces 
  - access modifiers etc.
- Compile-time errors_
@ulend



---
@title[What is TypeScript?]
### What is TypeScript?

TypeScript code is transpiled (for browsers) to JS at build time

![images/5_TS2JS.png](images/5_TS2JS.png)


---
@title[What is TypeScript?]
### TypeScript Primer Videos

We'll see video demonstrating these concepts:

@ul[list-bullets-black](true)
- type annotations
- arrow functions
- interfaces
- classes
- constructors
- access modifiers
- properties
- modules_
@ulend


---
@title[Contents]
### Video Slides

The following slides appear in the videos...


---
@title[Function Expressions]
### Function Expressions

@ul[](false)
- Function expressions have the following syntax:
@ulend

```javascript
var add = function(x,y)
{
  return x+y;
};

var ans = add(1,2); // ans=3
```

@ul[](true)
- The function above is actually an anonymous function assigned to variable ``add``
@ulend


---
@title[Function Declaration v Expression]
### Function Declaration v Expression

@ul[](true)
- They are more @size[1.5em](similar) than different
- You call them the same way
- They are just different @size[1.5em](styles) of writing functions
- But, you'll see function expression style more frequently from here
- Which one you chose is almost entirely a matter of personal taste
- But there are some differences...
@ulend


---
@title[Arrow Functions]
### Arrow Functions

@ul[](true)
- Arrow functions are an @size[1.5em](abbreviated) syntax for function expressions
- You don't need:
  - the ``function`` keyword
  - the ``return`` keyword
  - the curly brackets
- It's a new token **=>** 
- For example, let's look at the ``add()`` function again...
@ulend


---
@title[Access Modifiers]
### Access Modifiers

@ul[](true)
- public (default when not specified)
- private
- protected
@ulend








---?color=black
@title[Title]


@snap[west headline text-white span-70]
TypeScript
@snapend

@snap[south-west]
@fa[envelope-o pad-right-icon]@css[contact-email](thomas.devine@lyit.ie)
@snapend
