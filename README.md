# Angular Interview Questions & Answers
### Table of Contents

| No. | Questions |
| --- | --------- |
|1  | [What is Angular?](#what-is-angular) |
|2  | [What is 2 way binding?](#what-is-2-way-binding) |
|3  | [What is Angular lifecycle hooks?](#what-is-angular-lifecycle-hooks) |
|4  | [Which of the Angular life cycle component execution happens when a data bound input value updates?](#which-of-the-angular-life-cycle-component-execution-happens-when-a-data-bound-input-value-updates) |
|5  | [Differentiate between Components and Directives?](#differentiate-between-components-and-directives) |
|6  | [What is ng-content Directive?](#what-is-ng-content-directive) |
|7  | [What is service in angular?](#what-is-service-in-angular) |
|8  | [Why use interceptor or What is interceptor?](#why-use-interceptor-or-what-is-interceptor) |
|9  | [Differentiate between Observables and Promises](#differentiate-between-observables-and-promises) |
|10 | [What is Async pipes?](#what-is-async-pipes) |
|11 | [Features of typescript](#features-of-typescript ) |
|12 | [What is Aot compilation](#what-is-aot-compilation) |
|13 | [Providers in angular](#providers-in-angular) |
|14 | [What is Template refrence variable?](#what-is-template-refrence-variable) |
|15 | [Diffrence between Let Const and Var](#diffrence-between-let-const-and-var) |
|16 | [What is shared module?](#what-is-shared-module) |
|17 | [Angular Models](#angular-models) |
|18 | [What is Angular routes?](#what-is-angular-routes) |
|19 | [Diffrence between Subject and BehaviourSubject](#diffrence-between-subject-and-behavioursubject) | 




    
1. ### What is Angular?
 It is an open-source software engineering framework used for building single-page web apps. Developers also use it to create animated menus for HTML web pages.


   **[⬆ Back to Top](#table-of-contents)**
   
2. ### What is 2 way binding?
With two-way data binding, the framework (angular) is not only watching your variables for changes. It also keeps track of changes that are made by the user (for example with input-elements) and updates the variables accordingly.


**[⬆ Back to Top](#table-of-contents)**

3. ### What is Angular lifecycle hooks?
Angular 2 application goes through an entire set of processes or has a lifecycle right from its initiation to the end of the application.
ngOnChanges − When the value of a data bound property changes, then this method is called.

ngOnInit − This is called whenever the initialization of the directive/component after Angular first displays the data-bound properties happens.

ngDoCheck − This is for the detection and to act on changes that Angular can't or won't detect on its own.

ngAfterContentInit − This is called in response after Angular projects external content into the component's view.

ngAfterContentChecked − This is called in response after Angular checks the content projected into the component.

ngAfterViewInit − This is called in response after Angular initializes the component's views and child views.

ngAfterViewChecked − This is called in response after Angular checks the component's views and child views.

ngOnDestroy − This is the cleanup phase just before Angular destroys the directive/component.


**[⬆ Back to Top](#table-of-contents)**

4. ### Which of the Angular life cycle component execution happens when a data bound input value updates?
ngOnChanges is the life cycle hook that gets executed whenever a change happens to the data that was bound to an input.


**[⬆ Back to Top](#table-of-contents)**

5. ### Differentiate between Components and Directives?
Components have their own view (HTML and styles). Directives are just "behavior" added to existing elements and components.


**[⬆ Back to Top](#table-of-contents)**

6. ### What is ng-content Directive?
They are used to create configurable components. This means the components can be configured depending on the needs of its user. This is well known as Content Projection. Components that are used in published libraries make use of <ng-content> to make themselves configurable.
    
 
**[⬆ Back to Top](#table-of-contents)**

7. ### What is service in angular?.
A service is used when a common functionality needs to be provided to various modules. For example, we could have a database functionality that could be reused among various modules. And hence you could create a service that could have the database functionality.


**[⬆ Back to Top](#table-of-contents)**

8. ### Why use interceptor or What is interceptor?
Interceptors are a way to do some work for every single HTTP request or response.
--> Add a token or some custom HTTP header for all outgoing HTTP requests
--> Catch HTTP responses to do some custom formatting (i.e. convert CSV to JSON) before handing the data over to your service/component
--> Log all HTTP activity in the consol

**[⬆ Back to Top](#table-of-contents)**

9. ### Differentiate between Observables and Promises.
The first difference is that a Promise is eager, whereas an Observable is lazy.
If you create an Observable, you provide a callback function that will be called upon invoking subscribe method on the Observable object.
The next difference is that a Promise object may provide only a single value. It can be an array but it’s still a single object. On the contrary, an Observable may emit multiple values over time.
The most astonishing feature of the RxJS library is a great number of operators that can be applied to Observables in order to get a new tailored stream.

**[⬆ Back to Top](#table-of-contents)**


10. ### What is Async pipes?
The angular async pipe allows the subscription to observables inside of the angular template syntax. It also takes care of unsubscribing from observables automatically.

<p>{{ observable | async }}</p>

**[⬆ Back to Top](#table-of-contents)**


11. ### Features of typescript.
Object-Oriented language: TypeScript provides a complete feature of an object-oriented programming language such as classes, interfaces, inheritance, modules, etc. In TypeScript, we can write code for both client-side as well as server-side development.

TypeScript supports JavaScript libraries: TypeScript supports each JavaScript elements. It allows the developers to use existing JavaScript code with the TypeScript. Here, we can use all of the JavaScript frameworks, tools, and other libraries easily.

JavaScript is TypeScript: It means the code written in JavaScript with valid .js extension can be converted to TypeScript by changing the extension from .js to .ts and compiled with other TypeScript files.

TypeScript is portable: TypeScript is portable because it can be executed on any browsers, devices, or any operating systems. It can be run in any environment where JavaScript runs on. It is not specific to any virtual-machine for execution.

DOM Manipulation: TypeScript can be used to manipulate the DOM for adding or removing elements similar to JavaScript.

TypeScript is just a JS: TypeScript code is not executed on any browsers directly. The program written in TypeScript always starts with JavaScript and ends with JavaScript. Hence, we only need to know JavaScript to use it in TypeScript. The code written in TypeScript is compiled and converted into its JavaScript equivalent for the execution. This process is known as Trans-piled. With the help of JavaScript code, browsers can read the TypeScript code and display the output.

**[⬆ Back to Top](#table-of-contents)**

12. ### What is Aot compilation?
 If we compile the angular application with AOT mode, then it performs compilation of the templates with the help of the compiler and then generates the typescript files (file names like *ngfactory.ts, where * represents the actual name of the file, for example, if the component name is employee.ts then the related file will be employee.ngfactory.ts). Then compiler again compiles these typescript files to the JavaScript files.

In this compilation process, also a new type of file (*.metadata.json) has been created for every typescript files. These metadata files are required to compile the components for their templates. So, AOT Compiler validates the HTML templates at the build time and also raises an error if it finds any issues in our coding. 

**[⬆ Back to Top](#table-of-contents)**


13. ### Providers in angular.
In order for a service in Angular 2+ to be properly injected, it needs to be provided to either the component, the parent module or the app module. A service provided in the app module will have the same instance provided everywhere. Here's an example of two services provided in a component.

**[⬆ Back to Top](#table-of-contents)**


14. ### What is Template refrence variable?
    A template reference variable is often a reference to a DOM element within a template. It can also be a reference to an     Angular component or directive or a web component (Read more at Angular.io). That means you can easily access the           variable anywhere in the template.

    You declare a reference variable by using the hash symbol (#). The #firstNameInput declares a firstNameInput variable on        an <input> element.

            <input type="text" #firstNameInput>
            <input type="text" #lastNameInput>

    After that, you can access the variable anywhere inside the template. For example, I pass the variable as a parameter on        an event.

            <button (click)="show(lastNameInput)">Show</button>

**[⬆ Back to Top](#table-of-contents)**


15. ### Diffrence between Let Const and Var.

Scope of var

Scope essentially means where these variables are available for use. var declarations are globally scoped or function/locally scoped. It is globally scoped when a var variable is declared outside a function. This means that any variable that is declared with var outside a function block is available for use in the whole window. var is function scoped when it is declared within a function. This means that it is available and can be accessed only within that function

let is block scoped

A block is chunk of code bounded by {}. A block lives in curly braces. Anything within curly braces is a block. So a variable declared in a block with the let is only available for use within that block

const declarations are block scoped

Like let declarations, const declarations can only be accessed within the block it was declared.

const cannot be updated or re-declared

This means that the value of a variable declared with const remains the same within its scope. It cannot be updated or re-declared

**[⬆ Back to Top](#table-of-contents)**


16. ### What is shared module?
The scenario where you need to create a component that is going to be use on different modules of your application is quite usual that component will be part of shared module.

**[⬆ Back to Top](#table-of-contents)**


17. ### Angular Models

**[⬆ Back to Top](#table-of-contents)**


18. ### What is Angular routes?
 Router uses to navigate between views or pages that trigger by the user actions. Its a standard behavior in the web application, PWA, or Mobile Apps. The navigation or view changes happen when the user clicks on the link, click on the button, or enter the URL from the browser address bar. Every view change can bring the params of data from the previous view to the next view.

**[⬆ Back to Top](#table-of-contents)**


19. ### Diffrence between Subject and BehaviourSubject.
A BehaviorSubject holds one value. When it is subscribed it emits the value immediately. A Subject doesn't hold a value.

Subject example (with RxJS 5 API):

const subject = new Rx.Subject();
subject.next(1);
subject.subscribe(x => console.log(x));
Console output will be empty

BehaviorSubject example:

const subject = new Rx.BehaviorSubject();
subject.next(1);
subject.subscribe(x => console.log(x));

**[⬆ Back to Top](#table-of-contents)**
