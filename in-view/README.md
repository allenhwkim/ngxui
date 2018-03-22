# nguiInView
Utilize HTML5 IntersectionObserver 

- Observer callback does;
    * when isIntersecting (visible)?
        * load component
        * emit “nguiInview”
    * when not isIntersecting (not visible)?
        * unload component
        * emit “nguiNotInView”
    * execute transitionFn

## Input
* [nguiInViewOptions]=“object” 
    * [root](https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API#Intersection_observer_options)
    * [rootMargin](https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API#Intersection_observer_options)
    * [threshold](https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API#Intersection_observer_options)
    * transitionFn,  a function, default change opacity by 2% between 0 - 50%.

## Outputs
* (nguiInView)=“doSomething()” 
* (nguiNotInView)=“doSomething()”

## IntersectionObserver Browser Support
 - Chrome 51+
 - Edge 15+
 - Firefox 55+
 - IE11 N/A. Please use Polyfill  
   `<script src="https://polyfill.io/v2/polyfill.min.js?features=IntersectionObserver"></script>`
 - Opera 38+


