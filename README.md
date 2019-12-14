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
[10 | [What is Async pipes?](#what-is-async-pipes) |



    
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


10.What is Async pipes?

