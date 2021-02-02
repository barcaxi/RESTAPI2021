---?color=black
@title[Title]

@snap[west headline text-white span-70]
Angular
@snapend

@snap[south-west]
@fa[envelope-o pad-right-icon]@css[contact-email](thomas.devine@lyit.ie)
@snapend


---
@title[What is Angular?]
### What is Angular?

> Angular is a framework for building client applications using HTML, CSS, and TypeScript

---
@title[What is Angular?]
### Why Angular?

@ul[list-bullets-black](true)
- Angular provides a way to properly @size[1.25em](structure) our applications
- Angular makes web application development @size[1.25em](easier)
- Angular has a lot of @size[1.25em](reusable code)
- Angular applications are more @size[1.25em](testable)
- Angular allows us to write web app @size[1.5em](components)_
@ulend



---
@title[Angular Architecture]
### Angular Architecture

![images/1_architecture.png](images/1_architecture.png)

- Angular is used to build client front-end


---
@title[Angular Setup]
### Angular Setup

You will need:
@ul[list-bullets-black](true)
- Latest version of [Node](https://nodejs.org/en/)
- Angular CLI (Command Line Interface)
- Angular CLI creates new:
  - projects
  - components
  - services_
@ulend

---
@title[First Angular App]
### Angular App/Project - Hello Angular

```
$ ng new hello-world
  ...
$
```

---

@title[Modules & Components]
### Modules & Components


> Modules & Components are core concepts of Angular Apps

---

@title[Modules & Components]
### What are Components?

@ul[list-bullets-black](true)
- Every Angular App has at least one component
  - `AppComponent`
- But there are usually more than one component_
@ulend



---
### What are Components?

Each Component has its own -
![images/component0.png](images/component0.png)

@ul[list-bullets-black](true)
- Let's see some components for a website example...
@ulend

---
<!-- ### What are Components? -->

![images/component1.png](images/component1.png)

@ul[list-bullets-black](true)
- We could have ONE component...
@ulend


---
<!-- ### What are Components? -->

![images/component2.png](images/component2.png)

@ul[list-bullets-black](true)
- We could have these components...
@ulend

---
<!-- ### What are Components? -->

![images/component3.png](images/component3.png)

@ul[list-bullets-black](true)
- More component examples...
@ulend


---
<!-- ### What are Components? -->

![twitter0](images/twitter0.jpg)


---
### Components

Every Angular App has at least the `AppComponent` or *root* component...

![images/component4.png](images/component4.png)


---
### Components

...with a tree of Components within it.

![images/component5.png](images/component5.png)



---

@title[Modules & Components]
### What are Modules?

> a @size[1.5em](module) is a container for one or more related @size[1.5em](components)

---
@title[Modules & Components]
### What are Modules?

@ul[list-bullets-black](true)
- Every Angular App has at least one module:
  - the `AppModule`
  - or root module
- Modules are used to organise/store related components 
- So an App may have a number of modules that are containers for a number of related components
- Let's see an example...
@ulend

---
@title[Modules & Components]

![images/twitter1.jpg](images/twitter1.jpg)


---
@title[Modules & Components]

![images/twitter2.jpg](images/twitter2.jpg)


---
@title[Modules & Components]

![images/twitter3.jpg](images/twitter3.jpg)


---
@title[Creating Components]
### Creating Components

@ul[list-bullets-black](true)
- @size[1.5em](Components) are at the core of Angular
- We'll look at 2 ways of creating a Component
@ulend

@ol[list-bullets-black](true)
- Manual Component Creation within the editor
- Automatic Component Creation with Angular CLI
@olend

---
@title[Manual Component Creation]
### Manual Component Creation

3 steps:
@ol[list-bullets-black](true)
- Create the Component
- Register within a Module
- Add an element in HTML markup
@olend

---
@title[Component Creation with CLI]
### Component Creation with CLI

Create a new artist Component:

```
$ ng g c artist  // ng (g)enerate (c)omponent artist
  ...
$
```

@ol[list-bullets-black](true)
- Creates an new component folder - `app/artist`
- Registers the Component in `app/app.module.ts`
@olend



---
### Template Interpolation

> @size[1.5em](Interpolation) is the embedding of a TypeScript expression within a template

---
### Template Interpolation

```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-players',  
  template: `<h1>1 + 1 = {{ 1+1 }}</h1>`,
  styleUrls: ['./players.component.css']
})
export class PlayersComponent implements OnInit {
  player = "Messi";
}
```
@[5]()
@[*]()

---
### Template Interpolation

```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-players',  
  template: `<h1>{{ player }}</h1>`,
  styleUrls: ['./players.component.css']
})
export class PlayersComponent implements OnInit {
  player = "Messi";
}
```
@[5]()
@[*]()

---
### Dependency Injection

> @size[1.5em](Dependency Injection) is an important design pattern used in Angular

@ul[list-bullets-black](true)
- Dependencies are @size[1.5em](services) or @size[1.5em](objects) a class needs to perform its function
- The class asks for dependencies from external sources rather than creating them itself
@ulend


---

Dependencies are services or objects that a class needs to perform its function. DI is a coding pattern in which a class asks for dependencies from external sources rather than creating them itself.


---
@title[Dislay Data & Event Handling]
### Display Data & Event Handling

Topics
@ul[list-bullets-black](true)
- Event Handling
- Property Binding
- Two way binding 
@ulend


---
@title[Title]

### Two-way Binding

> The `ngmodel` directive binds the value of HTML controls (input, select, textarea) to Component data.


---

### Pipes

> A pipe takes in data as input and transforms it to a desired output

---

### Pipes

Angular has a selection of pipes such as:
@ul[list-bullets-black](true)
- Date Pipe
- UpperCase Pipe
- LowerCase Pipe 
- Currency Pipe
- Percent Pipe_
@ulend


---
@title[Directives]
### Directives


@ul[list-bullets-black](true)
- ngIf
- ngFor
- ngSwitchCase
- ngClass
- ngStyle
@ulend



---
@title[Directives]
<!-- ### Directives -->

![images/directives.png](images/directives.png)

---
@title[ngFor]
### ngFor export values

@ul[list-bullets-black](true)
- index: number - index of the current item
- first: boolean - `true` when the item is the first item 
- last: boolean - `true` when the item is the last item 
- even: boolean: `true` when the item has an even index 
- odd: boolean: `true` when the item has an odd index 
@ulend

---
@title[FormControl]
<!-- ### Directives -->

![images/6_formControl.png](images/6_formControl.png)


---
@title[FormControl]
<!-- ### Directives -->

![images/6_formControl.png](images/6_formControl2.png)


---
@title[FormControl]
<!-- ### Directives -->

![images/8_form.png](images/8_form.png)


---
@title[HTTP Services]
<!-- ### HTTP Services -->

![images/ClientServerArchitecture.png](images/ClientServerArchitecture.png)

---
@title[HTTP Services]
<!-- ### HTTP Services -->

![images/HTTPRequests.png](images/HTTPRequests.png)

---
@title[SOC]
### Separation of Concerns

![images/SOC1.png](images/SOC1.png)

---
@title[SOC]
### Separation of Concerns

![images/SOC2.png](images/SOC2.png)


---
@title[routerModule]
<!-- ### Router Module -->

![images/SOC2.png](images/routerModule.png)


---?color=black
@title[Title]


@snap[west headline text-white span-70]
Angular
@snapend

@snap[south-west]
@fa[envelope-o pad-right-icon]@css[contact-email](thomas.devine@lyit.ie)
@snapend
