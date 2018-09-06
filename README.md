# Vue JS 2: From Beginner to Professional 

This repository contains the excercises of the udemy course:
 [Vue JS 2: From Beginner to Professional](https://www.udemy.com/vuejs-from-beginner-to-professional/).
 
 <b>Table of Contents</b>
 
 * Hello World
 * Template
    * Expression
    * If
    * Function
    
 * Methods
    * Basic property
    * Property with parameters
    * Property and objects
    
 * Arrow function

        Remember: Be aware that the arrow functions can have 
        strange behavior so, don't use that inside the Vue instance
        
For example:
```$xslt
new Vue({
            el: '#app',
            data: {
                name: 'Simone',
                surname: 'Biffi'
            },
            methods: {
                getFullName: function (first, last) {
                    return this.first + ' ' + this.last
                }
            }
        })
```
In this snippet the <b>getFullName</b> property return <b>undefined undefined</b> because 
the object <b>this</b> refers to the whole page and not to the Vue object.

* Directives
    
    We can't use datas inside html attributes son we use directive to bind this or also to perform other actions.
    * Basic directives 