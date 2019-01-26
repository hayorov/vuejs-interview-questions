# vuejs-interview-questions
List of 300 VueJS Interview Questions

> Click :star:if you like the project. Pull Request are highly appreciated.

### Table of Contents
-------------------------------------------------------------------
| No. | Questions |
|---- | ---------
|1  | [What is VueJS](#what-is-vuejs) |
|2  | [What are the major features of VueJS](#what-are-the-major-features-of-vuejs) |
|3  | [What are the lifecycle methods of VueJS](#what-are-the-lifecycle-methods-of-vuejs)|
|4  | [What are the conditional directives](#what-are-the-conditional-directives)|
|5  | [What is the difference between v-show and v-if directives](#what-is-the-difference-between-v-show-and-v-if-directives)|
|6  | [What is the purpose of v-for directive?](#what-is-the-purpose-of-v-for-directive)|
|7  | [What is vue instance?](#what-is-vue-instance)|
|8  | [How do you achieve conditional group of elements?](#how-do-you-achieve-conditional-group-of-elements)|
|9  | [How do you reuse elements with key attribute?](#how-do-you-reuse-elements-with-key-attribute)|
|10 | [Why should not use if and for directives together on the same element?](#why-should-not-use-if-and-for-directives-together-on-the-same-element)|
|11 | [Why do you need to use key attribute on for directive?](#why-do-you-need-to-use-key-attribute-on-for-directive)|
|12 | [What are the array detection mutation methods?](#what-are-the-array-detection-mutation-methods)|
|13 | [What are the array detection non mutation methods?](#what-are-the-array-detection-non-mutation-methods)|
|14 | [What are the caveats of array changes detection?](#what-are-the-caveats-of-array-changes-detection)|
|15 | [What are the caveats of object changes detection?](#what-are-the-caveats-of-object-changes-detection)|
|16 | [How do you use for directive with a range?](#how-do-you-use-for-directive-with-a-range)|
|17 | [How do you use for directive on template?](#how-do-you-use-for-directive-on-template)|
|18 | [How do you use event handlers?](#how-do-you-use-event-handlers)|
|19 | [What are the event modifiers provided by vue?](#what-are-the-event-modifiers-provided-by-vue)|
|20 | [What are key modifiers?](#what-are-key-modifiers)|
|21 | [How do you define custom key modifier aliases?](#how-do-you-define-custom-key-modifier-aliases)|
|22 | [What are the supported System Modifier Keys?](#what-are-the-supported-system-modifier-keys)|
|23 | [What are the supported Mouse Button Modifiers?](#what-are-the-supported-mouse-button-modifiers)|
|24 | [How do you implement two way binding?](#how-do-you-implement-two-way-binding)|
|25 | [What are the supported modifiers on model?](#what-are-the-supported-modifiers-on-model)|
|26 | [What are components and give an example?](#what-are-components-and-give-an-example)|
|27 | [What are props?](#what-are-props)|
|28 | [When component needs a single root element?](#when-component-needs-a-single-root-element)|
|29 | [How do you communicate from child to parent using events?](#how-do-you-communicate-from-child-to-parent-using-events)|
|30 | [How do you implement model on custom input components?](#how-do-you-implement-model-on-custom-input-components)|
|31 | [What are slots?](#what-are-slots)|
|32 | [What is global registration in components?](#what-is-global-registration-in-components)|
|33 | [Why do you need local registration?](#why-do-you-need-local-registration)|
|34 | [What is the difference between local and global registration in module system?](#what-is-the-difference-between-local-and-global-registration-in-module-system)|
|35 | [What are possible prop types?](#what-are-possible-prop-types)|
|36 | [What is the data flow followed by props?](#what-is-the-data-flow-followed-by-props)|
|37 | [What are non prop attributes?](#what-are-non-prop-attributes)|
|38 | [Describe about validations available for props?](#describe-about-validations-available-for-props)|
|39 | [How do you customize model directive for a component?](#how-do-you-customize-model-directive-for-a-component)|
|40 | [What are the possible ways to provide transitions?](#What-are-the-possible-ways-to-provide-transitions)|
|41 | [What is vue router and their features?](#what-is-vue-router-and-their-features)|
|42 | [What are the steps to use vue router and give an example?](#what-are-the-steps-to-use-vue-router-and-give-an-example)|
|43 | [What is dynamic route matching?](#what-is-dynamic-route-matching)|
|44 | [How to make router param changes as reactive?](#how-to-make-router-param-changes-as-reactive)|
|45 | [What is route matching priority?](#what-is-route-matching-priority)|
|46 | [What are nested routes?](#what-are-nested-routes)|
|47 | [What are single file components?](#what-are-single-file-components)|
|48 | [Is Single File Components violating separation of concerns?](#is-single-file-components-violating-separation-of-concerns)|
|49 | [What are the problems solved by Single File Components?](#what-are-the-problems-solved-by-single-file-components)|
|50 | [What are filters?](#what-are-filters)|
|51 | [What are the different ways to create filters?](#what-are-the-different-ways-to-create-filters)|
|52 | [How do you chain filters](#how-do-you-chain-filters)|
|53 | [Is it possible to pass parameters for filters?](#is-it-possible-to-pass-parameters-for-filters)|
|54 | [What are plugins and their various services?](#what-are-plugins-and-their-various-services)|
|55 | [ How to create a plugin?](#how-to-create-a-plugin)|
|56 | [How to use a plugin?](#how-to-use-a-plugin)|

1.  ### What is VueJS?
    Vue.js is an open-source, progressive Javascript framework for building user interfaces that aim to be incrementally adoptable. The core library of VueJS is focused on the view layer only, and is easy to pick up and integrate with other libraries or existing projects.
2.  ### What are the major features of VueJS?
    Below are the some of major features available with VueJS
    1. **Virtual DOM:** It uses virtual DOM similar to other existing frameworks such as ReactJS, Ember etc. Virtual DOM is a light-weight in-memory tree representation of the original HTML DOM and updated without affecting the original DOM.
    2. **Components:** Used to create reusable custom elements in VueJS applications.
    3. **Templates:** VueJS provides HTML based templates that bind the DOM with the Vue instance data
    4. **Routing:** Navigation between pages is achieved through vue-router
    5. **Light weight:** VueJS is light weight library compared to other frameworks
3.  ### What are the lifecycle methods of VueJS?
    Lifecycle hooks are a window into how the library you’re using works behind-the-scenes. By using these hooks, you will know when your component is created, added to the DOM, updated, or destroyed. Let's look at lifecycle diagram before going to each lifecycle hook in detail,

    <img src="https://github.com/sudheerj/vuejs-interview-questions/blob/master/images/vuelifecycle.png" width="400" height="800">

    1. **Creation(Initialization):**
        Creation Hooks allow you to perform actions before your component has even been added to the DOM. You need to use these hooks if you need to set things up in your component both during client rendering and server rendering. Unlike other hooks, creation hooks are also run during server-side rendering.
        1. beforeCreate:
           This hook runs at the very initialization of your component. hook observes data and initialization events in your component. Here, data is still not reactive and events that occur during the component’s lifecycle have not been set up yet.
        ```javascript
            new Vue({
              data: {
               count: 10
              },
              created: function () {
                console.log('Nothing gets called at this moment')
                // `this` points to the view model instance
                console.log('count is ' + this.count);
              }
            })
               // count is undefined
         ```
        2. created:
            This hook is invoked when Vue has set up events and data observation. Here, events are active and access to reactive data is enabled though templates have not yet been mounted or rendered.
        ```javascript
          new Vue({
            data: {
             count: 10
            },
            created: function () {
              // `this` points to the view model instance
              console.log('count is: ' + this.count)
            }
          })
             // count is: 10
        ```
        **Note:** Remember that, You will not have access to the DOM or the target mounting element (this.$el) inside of creation hooks
    2. **Mounting(DOM Insertion):**
        Mounting hooks are often the most-used hooks and they allow you to access your component immediately before and after the first render.
        1. beforeMount:
            They allow you to access your component immediately before and after the first render.
        ```javascript
          new Vue({
            beforeMount: function () {
              // `this` points to the view model instance
              console.log(`this.$el is yet to be created`);
            }
          })
        ```
        2. mounted:
            This is a most used hook and you will have full access to the reactive component, templates, and rendered DOM (via. this.$el).  The most frequently used patterns are fetching data for your component.
        ```javascript
        <div id="app">
            <p>I'm text inside the component.</p>
        </div>
          new Vue({
            el: '#app',
            mounted: function() {
              console.log(this.$el.textContent); // I'm text inside the component.
            }
          })
        ```
    3. **Updating (Diff & Re-render):**
        Updating hooks are called whenever a reactive property used by your component changes, or something else causes it to re-render
        1. beforeUpdate:
        The beforeUpdate hook runs after data changes on your component and the update cycle begins, right before the DOM is patched and re-rendered.
        ```javascript
        <div id="app">
          <p>{{counter}}</p>
        </div>
        ...// rest of the code
          new Vue({
            el: '#app',
            data() {
              return {
                counter: 0
              }
            },
             created: function() {
              setInterval(() => {
                this.counter++
              }, 1000)
            },

            beforeUpdate: function() {
              console.log(this.counter) // Logs the counter value every second, before the DOM updates.
            }
          })
        ```
        2. updated:
            This hook runs after data changes on your component and the DOM re-renders.
        ```javascript
        <div id="app">
          <p ref="dom">{{counter}}</p>
        </div>
        ...//
          new Vue({
            el: '#app',
            data() {
              return {
                counter: 0
              }
            },
             created: function() {
              setInterval(() => {
                this.counter++
              }, 1000)
            },
            updated: function() {
              console.log(+this.$refs['dom'].textContent === this.counter) // Logs true every second
            }
          })
        ```
    4. **Destruction (Teardown):**
        Destruction hooks allow you to perform actions when your component is destroyed, such as cleanup or analytics sending.
        1. beforeDestroy:
        `beforeDestroy` is fired right before teardown. If you need to cleanup events or reactive subscriptions, beforeDestroy would probably be the time to do it. Your component will still be fully present and functional.
        ```javascript
        new Vue ({
          data() {
            return {
              message: 'Welcome VueJS developers'
            }
          },

          beforeDestroy: function() {
            this.message = null
            delete this.message
          }
        })
        ```
        2. destroyed:
        This hooks is called after your component has been destroyed, its directives have been unbound and its event listeners have been removed.
        ```javascript
        new Vue ({
            destroyed: function() {
              console.log(this) // Nothing to show here
            }
          })
        ```

4.  ### What are the conditional directives?
    VueJS provides set of directives to show or hide elements based on conditions. The available directives are: ** v-if, v-else, v-else-if and v-show**
    **1. v-if:**  The v-if directive adds or removes DOM elements based on the given expression. For example, the below button will not show if isLoggedIn is set to false.
    ```javascript
    <button v-if="isLoggedIn">Logout</button>
    ```
    You can also control multiple elements with a single v-if statement by wrapping all the elements in a <template> element with the condition. For example, you can have both label and button together conditionally applied,
    ```javascript
    <template v-if="isLoggedIn">
      <label> Logout </button>
      <button> Logout </button>
    </template>
    ```
    **2. v-else:**  This directive is used to display content only when the expression adjacent v-if resolves to false. This is similar to else block in any programming language to display alternative content and it is preceded by v-if or v-else-if block. You don't need to pass any value to this.
    For example, v-else is used to display LogIn button if isLoggedIn(not logged in) is set to false.
    ```javascript
    <button v-if="isLoggedIn"> Logout </button>
    <button v-else> Log In </button>
    ```
    **3. v-else-f:** This directive is used when we need more than two options to be checked.
    For example, ifLoginDisabled property is disabled then we need to prevent user to login instead just display the label. This can be achieved through v-else statement.
    ```javascript
    <button v-if="isLoggedIn"> Logout </button>
    <label v-else-if="isLoginDisabled"> User login disabled </label>
    <button v-else> Log In </button>
    ```

    **4. v-show:** This directive is similar to v-if but it renders all elements to the DOM and then uses the CSS display property to show/hide elements. This directive is recommended if the elements are switched on and off frequently.
    ```javascript
    <span if-show="user.name">Welcome user,{{user.name}}</span>
    ```
5.  ### What is the difference between v-show and v-if directives?
    Below are some of the main differences between between **v-show** and **v-if** directives,
        1. v-if only renders the element to the DOM if the expression passes whereas v-show renders all elements to the DOM and then uses the CSS display property to show/hide elements based on expression.
        2. v-if supports v-else and v-else-if directives whereas v-show doesn't support else directives.
        3. v-if has higher toggle costs while v-show has higher initial render costs. i.e, v-show has a performance advantage if the elements are switched on and off frequently, while the v-if has the advantage when it comes to initial render time.
        4. v-if supports <template> tab but v-show doesn't support.
6.  ### What is the purpose of v-for directive?
    The built-in v-for directive allows us to loop through items in an array or object. You can iterate on each element in the array or object.
    1. Array usage:
    ```javascript
    <ul id="list">
      <li v-for="(item, index) in items">
        {{ index }} - {{ item.message }}
      </li>
    </ul>

    var vm = new Vue({
      el: '#list',
      data: {
        items: [
          { message: 'John' },
          { message: 'Locke' }
        ]
      }
    })
    ```
    You can also use `of` as the delimiter instead of `in`, similar to javascript iterators.
    2. Object usage:
    ```javascript
    <div id="object" v-for="(value, key, index) in object">
      {{ index }}. {{ key }}: {{ value }}
    </div>

    var vm = new Vue({
      el: '#object',
      data: {
        user: {
          firstName: 'John',
          lastName: 'Locke',
          age: 30
        }
      }
    })
    ```
7.  ### What is vue instance?
    Every Vue application works by creating a new Vue instance with the Vue function. Generally the variable vm (short for ViewModel) is used to refer Vue instance. You can create vue instance as below,
    ```javascript
    var vm = new Vue({
      // options
    })
    ```
    As mentioned in the above code snippets, you need to pass options object. You can find the full list of options in the API reference.
8.  ### How do you achieve conditional group of elements?
    You can achieve conditional group of elements(toggle multiple elements at a time) by applying **v-if** directive on `<template>` element which works as invisible wrapper(no rendering) for group of elements. For example, you can conditionally group user details based on valid user condition
    ```javascript
    <template v-if="condition">
      <h1>Name</h1>
      <p>Address</p>
      <p>Contact Details</p>
    </template>
    ```
9.  ### How do you reuse elements with key attribute?
    Vue always try to render elements as efficient as possible. So it tries to reuse the elements instead of building them from scratch. But this behavior may cause problems in few scenarios. For example, if you try to render the same input element in both `v-if` and `v-else` blocks then it holds the previous value as below,
    ```javascript
    <template v-if="loginType === 'Admin'">
      <label>Admin</label>
      <input placeholder="Enter your ID">
    </template>
    <template v-else>
      <label>Guest</label>
      <input placeholder="Enter your name">
    </template>
    ```
    In this case, it shouldn't reuse. We can make both input elements as separate by applying **key** attribute as below,
    ```javascript
        <template v-if="loginType === 'Admin'">
          <label>Admin</label>
          <input placeholder="Enter your ID" key="admin-id">
        </template>
        <template v-else>
          <label>Guest</label>
          <input placeholder="Enter your name" key="user-name">
        </template>
    ```
    The above code make sure both inputs are independent and doesn't impact each other.
10. ### Why should not use if and for directives together on the same element?
    It is recommended not to use v-if on the same element as v-for. Because v-for directive has a higher priority than v-if. There are two cases where developers try to use this combination,
    1. To filter items in a list
     For example, if you try to filter the list using v-if tag,
     ```javascript
     <ul>
       <li
         v-for="user in users"
         v-if="user.isActive"
         :key="user.id"
       >
         {{ user.name }}
       <li>
     </ul>
     ```
     This can be avoided by preparing the filtered list using computed property on the initial list
     ```javascript
     computed: {
       activeUsers: function () {
         return this.users.filter(function (user) {
           return user.isActive
         })
       }
     }
     ...... //
     ...... //
     <ul>
       <li
         v-for="user in activeUsers"
         :key="user.id">
         {{ user.name }}
       <li>
     </ul>

     ```
    2. To avoid rendering a list if it should be hidden
     For example, if you try to conditionally check if the user is to show or hide
     ```javascript
     <ul>
       <li
         v-for="user in users"
         v-if="shouldShowUsers"
         :key="user.id"
       >
         {{ user.name }}
       <li>
     </ul>
     ```
     This can be solved by moving the condition to a parent by avoiding this check for each user
     ```javascript
     <ul v-if="shouldShowUsers">
       <li
         v-for="user in users"
         :key="user.id"
       >
         {{ user.name }}
       <li>
     </ul>
     ```
11.  ### Why do you need to use key attribute on for directive?
     In order to track each node’s identity, and thus reuse and reorder existing elements, you need to provide a unique `key` attribute for each item with in `v-for` iteration. An ideal value for key would be the unique id of each item. Let us take an example usage,
     ```javascript
     <div v-for="item in items" :key="item.id">
       {{item.name}}
     </div>
     ```
     Hence, It is always recommended to provide a key with v-for whenever possible, unless the iterated DOM content is simple.
     **Note:** You shouldn’t use non-primitive values like objects and arrays as v-for keys. Use string or numeric values instead.
12.  ### What are the array detection mutation methods?
     As the name suggests, mutation methods modifies the original array. Below are the list of array mutation methods which trigger view updates.
     1. push()
     2. pop()
     3. shift()
     4. unshift()
     5. splice()
     6. sort()
     7. reverse()
     If you perform any of the above mutation method on the list then it triggers view update. For example, push method on array named 'items' trigger a view update,
     ```javascript
     vm.todos.push({ message: 'Baz' })
     ```
13.  ### What are the array detection non mutation methods?
     The methods which do not mutate the original array but always return a new array are called non-mutation methods. Below are the list of non-mutation methods,
     1. filter()
     2. concat()
     3. slice()
     For example, lets take a todo list where it replaces the old array with new one based on status filter,
     ```javascript
     vm.todos = vm.todos.filter(function (todo) {
       return todo.status.match(/Completed/)
     })
     ```
     This approach won't re-render the entire list due to VueJS implementation.
14.  ### What are the caveats of array changes detection?
     Vue cannot detect changes for the array in the below two cases,

     1. When you directly set an item with the index,For example,
        ```javascript
        vm.tods[indexOfTodo] = newTodo
        ```
     2. When you modify the length of the array, For example,
      ```javascript
      vm.todos.length = todosLength
      ```
     You can overcome both the caveats using `set` and `splice` methods, Let's see the solutions with an examples,
     **First use case solution**
     ```javascript
     // Vue.set
     Vue.set(vm.todos, indexOfTodo, newTodoValue)
     (or)
     // Array.prototype.splice
     vm.todos.splice(indexOfTodo, 1, newTodoValue)
     ```
     **Second use case solution**
     ```javascript
     vm.todos.splice(todosLength)
     ```
15.  ### What are the caveats of object changes detection?
     Vue cannot detect changes for the object in property addition or deletion., Lets take an example of user data changes,
     ```javascript
     var vm = new Vue({
       data: {
         user: {
           name: 'John'
         }
       }
     })

     // `vm.name` is now reactive

     vm.email = john@email.com // `vm.email` is NOT reactive
     ```
     You can overcome this scenario using the Vue.set(object, key, value) method or Object.assign(),
     ```javascript
     Vue.set(vm.user, 'email', john@email.com);
     (or)
     vm.user = Object.assign({}, vm.user, {
       email: john@email.com
     })
     ```
16.  ### How do you use for directive with a range?
     You can also use integer type(say 'n') for v-for directive which repeat the element many times.
     ```javascript
     <div>
       <span v-for="n in 20">{{ n }} </span>
     </div>
     ```
     It displays the number 1 to 20.
17.  ### How do you use for directive on template?
     Just similar to v-if directive on template, you can also use a <template> tag with v-for directive to render a block of multiple elements. Let's take a todo example,
     ```javascript
     <ul>
       <template v-for="todo in todos">
         <li>{{ todo.title }}</li>
         <li class="divider"></li>
       </template>
     </ul>
     ```
18.  ### How do you use event handlers?
     You can use event handlers in vue similar to plain javascript. The method calls also support the special $event variable.
     ```javascript
     <button v-on:click="show('Welcome to VueJS world', $event)">
       Submit
     </button>

     \\\\
     methods: {
       show: function (message, event) {
         // now we have access to the native event
         if (event) event.preventDefault()
         console.log(message);
       }
     }
     ```
19.  ### What are the event modifiers provided by vue?
     Normally, javascript provides event.preventDefault() or event.stopPropagation() inside event handlers. You can use methods provided by vue, but these methods are meant for data logic instead of dealing with DOM events. Vue provides below event modifiers for v-on and these modifiers are directive postfixes denoted by a dot.
     1. .stop
     2. .prevent
     3. .capture
     4. .self
     5. .once
     6. .passive
     Let's take an example of stop modifier,
     ```javascript
     <!-- the click event's propagation will be stopped -->
     <a v-on:click.stop="methodCall"></a>
     ```
     You can also chain modifiers as below,
     ```javascript
     <!-- modifiers can be chained -->
     <a v-on:click.stop.prevent="doThat"></a>
     ```
20.  ### What are key modifiers?
     Vue supports key modifiers on `v-on` for handling keyboard events. Let's take an example of keyup event with enter keycode
     ```javascript
     <!-- only call `vm.show()` when the `keyCode` is 13 -->
     <input v-on:keyup.13="show">
     ```
     Remembering all the keycodes is really difficult. It supports the full list of keycode aliases
     1. .enter
     2. .tab
     3. .delete (captures both “Delete” and “Backspace” keys)
     4. .esc
     5. .space
     6. .up
     7. .down
     8. .left
     9. .right

     Now the above keyup code snippet can be written with aliases as follows,
     ```javascript
     <input v-on:keyup.enter="submit">
     (OR)
     <!-- with shorthand notation-->
     <input @keyup.enter="submit">
     ```
21.  ### How do you define custom key modifier aliases?
     You can define custom key modifier aliases via the global `config.keyCodes`. There are few guidelines for the properties
     1. You can't use cameCase, instead you can use kebab-case with double quotation marks
     2. You can define multiple values in ann array format
     ```javascript
     Vue.config.keyCodes = {
       f1: 112,
       "media-play-pause": 179,
       down: [40, 87]
     }
     ```
22.  ### What are the supported System Modifier Keys?
     Vue supports below modifiers to trigger mouse or keyboard event listeners when the corresponding key is pressed,
     1. .ctrl
     2. .alt
     3. .shift
     4. .meta
     Lets take an example of control modifier with click event,
     ```javascript
     <!-- Ctrl + Click -->
     <div @click.ctrl="doSomething">Do something</div>
     ```
23.  ### What are the supported Mouse Button Modifiers?
     Vue supports below mouse button modifiers
     1. .left
     2. .right
     3. .middle
     For example, the usage of `.right` modifier as below
     ```javascript
      <button v-if="button === 'right'"
                 v-on:mousedown.right="increment" v-on:mousedown.left="decrement" />
     ```
24.  ### How do you implement two way binding?
     You can use the `v-model` directive to create two-way data bindings on form input, textarea, and select elements. Lets take an example of it using input component,
     ```javascript
     <input v-model="message" placeholder="Enter innput here">
     <p>The message is: {{ message }}</p>
     ```
     Remember, v-model will ignore the initial value, checked or selected attributes found on any form elements. So it always use the Vue instance data as the source of truth.
25.  ### What are the supported modifiers on model?
     There are three modifiers supported for v-model directive.
     **1. lazy:** By default, v-model syncs the input with the data after each input event. You can add the lazy modifier to instead sync after change events.
     ```javascript
     <!-- synced after "change" instead of "input" -->
     <input v-model.lazy="msg" >
     ```
     **2. number:** If you want user input to be automatically typecast as a number, you can add the number modifier to your v-model. Even with type="number", the value of HTML input elements always returns a string. So, this typecast modifier is required.
     ```javascript
     <input v-model.number="age" type="number">
     ```
     **3. trim:** If you want whitespace from user input to be trimmed automatically, you can add the trim modifier to your v-model.
     ```javascript
     <input v-model.trim="msg">
     ```
26.  ### What are components and give an example?
     Components are reusable Vue instances with a name. They accept the same options as new Vue, such as data, computed, watch, methods, and lifecycle hooks(except few root-specific options like el). Lets take an example of counter component,
     ```javascript
     // Define a new component called button-counter
     Vue.component('button-counter', {
       template: '<button v-on:click="count++">You clicked me {{ count }} times.</button>'
       data: function () {
         return {
           count: 0
         }
       },
     })
     ```
     Let's use this component inside a root Vue instance created with new Vue
     ```javascript
     <div id="app">
       <button-counter></button-counter>
     </div>

     var vm = new Vue({ el: '#app' });
     ```
27.  ### What are props?
     Props are custom attributes you can register on a component. When a value is passed to a prop attribute, it becomes a property on that component instance. You can pass those list of values as props option and use them as similar to data variables in template.
     ```javascript
     Vue.component('todo-item', {
       props: ['title'],
       template: '<h2>{{ title }}</h2>'
     })
     ```
     Once the props registered, you can pass them as custom atrtributes,
     ```javascript
     <todo-item title="Learn Vue conceptsnfirst"></todo-item>
     ```
28.  ### When component needs a single root element?
     Every component must have a single root element when template has more than one element. In this case, you need to wrap a parent element.
     ```javascript
     <div class="todo-item">
       <h2>{{ title }}</h2>
       <div v-html="content"></div>
     </div>
     ```
     Otherwise there will an error throwing, saying that "wrap those elements with a parent element".
29.  ### How do you communicate from child to parent using events?
     If you want child wants to communicate back up to the parent, then emit an event from child using `$event` object to parent,
     ```javascript
     Vue.component('todo-tem', {
       props: ['todo'],
       template: `
         <div class="todo-item">
           <h3>{{ todo.title }}</h3>
           <button v-on:click="$emit('increment-count', 1)">
             Add
           </button>
           <div v-html="todo.description"></div>
         </div>
       `
     })
     ```
     Now you can use this todo-item in parent component to access the count value.
     ```javascript
     <ul v-for="todo in todos">
     <li>
        <todo-item
           v-bind:key="todo.id"
           v-bind:todo="todo" v-on:increment-count="total += 1"></todo-item>
     </li>
     </ul>
     <span> Total todos count is {{total}}</span>
     ```
30.  ### How do you implement model on custom input components?
     The custom events can also be used to create custom inputs that work with v-model. The <input> inside the component must follow below rules,
     1. Bind the value attribute to a value prop
     2. On input, emit its own custom input event with the new value.
     Lets take a custom-input component as an example,
     ```javascript
     Vue.component('custom-input', {
       props: ['value'],
       template: `
         <input
           v-bind:value="value"
           v-on:input="$emit('input', $event.target.value)"
         >
       `
     })
     ```
     Now you can use `v-model` with this component,
     ```javascript
     <custom-input v-model="searchInput"></custom-input>
     ```
31.  ### What are slots?
     Vue implements a content distribution API using the <slot> element to serve as distribution outlets for content created after after the current Web Components spec draft. Let's create ann alert component with slots for content insertion,
     ```javascript
     Vue.component('alert', {
       template: `
         <div class="alert-box">
           <strong>Error!</strong>
           <slot></slot>
         </div>
       `
     })
     ```
     Now you can insert dynamic content as below,
     ```javascript
     <alert>
       There is an issue with in application.
     </alert>
     ```
32.  ### What is global registration in components?
     The components which are globally registered can be used in the template of any root Vue instance (new Vue) created after registration. In the global registration, the components created using Vue.component as below,
     ```javascript
     Vue.component('my-component-name', {
       // ... options ...
     })
     ```
     Let's take multiple components which are globally registered in the vue instance,
     ```javascript
     Vue.component('component-a', { /* ... */ })
     Vue.component('component-b', { /* ... */ })
     Vue.component('component-c', { /* ... */ })

     new Vue({ el: '#app' })
     ```
     The above components can be used in the vue instance,
     ```javascript
     <div id="app">
       <component-a></component-a>
       <component-b></component-b>
       <component-c></component-c>
     </div>
     ```
     Remember that the components can be used in subcomponents as well.
33.  ### Why do you need local registration?
     Due to global registration, even if you don't use the component it could still be included in your final build. So it will create unnecessary javascript in the application. This can be avoided using local registration with the below steps,
     1. First you need to define your components as plain JavaScript objects
     ```javascript
     var ComponentA = { /* ... */ }
     var ComponentB = { /* ... */ }
     var ComponentC = { /* ... */ }
     ```
     Locally registered components will not be available in sub components. In this case, you need to add them in components section
     ```javascript
     var ComponentA = { /* ... */ }

     var ComponentB = {
       components: {
         'component-a': ComponentA
       },
       // ...
     }
     ```
     2. You can use the components in the components section of the vue instance,
     ```javascript
     new Vue({
       el: '#app',
       components: {
         'component-a': ComponentA,
         'component-b': ComponentB
       }
     })
     ```
34.  ### What is the difference between local and global registration in module system?
     In **local registration**, you need to create each component in components folder(optional but it is recommended) and import them in another component file components section. Let's say you want to register component A and B in component C, the configuration seems as below,
     ```javascript
     import ComponentA from './ComponentA'
     import ComponentB from './ComponentC'

     export default {
       components: {
         ComponentA,
         ComponentB
       },
       // ...
     }
     ```
     Now both ComponentA and ComponentB can be used inside ComponentC‘s template.

     In **global registration**, you need to export all common or base components in a separate file. But some of the popular bundlers like `webpack` make this process simpler by using `require.context` to globally register base components in the below entry file(one-time).

     ```javascript
     import Vue from 'vue'
     import upperFirst from 'lodash/upperFirst'
     import camelCase from 'lodash/camelCase'

     const requireComponent = require.context(
       // The relative path of the components folder
       './components',
       // Whether or not to look in subfolders
       false,
       // The regular expression used to match base component filenames
       /Base[A-Z]\w+\.(vue|js)$/
     )

     requireComponent.keys().forEach(fileName => {
       // Get component config
       const componentConfig = requireComponent(fileName)

       // Get PascalCase name of component
       const componentName = upperFirst(
         camelCase(
           // Strip the leading `./` and extension from the filename
           fileName.replace(/^\.\/(.*)\.\w+$/, '$1')
         )
       )

       // Register component globally
       Vue.component(
         componentName,
         // Look for the component options on `.default`, which will
         // exist if the component was exported with `export default`,
         // otherwise fall back to module's root.
         componentConfig.default || componentConfig
       )
     })
     ```
35.  ### What are possible prop types?
     You can declare props with type or without type. But it is recommended to have prop types because it provides the documentation for the component and warns the developer for any incorrect data type is assigned.
     ```javascript
     props: {
       name: String,
       age: Number,
       isAuthenticated: Boolean,
       phoneNumbers: Array,
       address: Object
     }
     ```
     As mentioned in the above code snippet, you can list props as an object, where the properties’ names and values contain the prop names and types, respectively.
36.  ### What is the data flow followed by props?
     All props follows a one-way-down binding between the child property and the parent one. i.e, When the parent property is updated then that latest prop value will be passed down to the child, but not the otherway(child to parent) around. The child component should not mutate the prop otherwise it throws a warning in the console.
     The possible mutation cases can be solved as below,
     1. When you try to use parent prop as initial value for child property:
     In this case you can define a local property in child component and assign parent value as initial value
     ```javascript
     props: ['defaultUser'],
     data: function () {
       return {
         username: this.defaultUser
       }
     }
     ```
     2. When you try to transform the parent prop:
     You can define a computed property using the prop’s value,
     ```javascript
     props: ['environment'],
     computed: {
       environment: function () {
         return this.environment.trim().toUpperCase()
       }
     }
     ```
37.  ### What are non prop attributes?
     A non-prop attribute is an attribute that is passed to a component, but does not have a corresponding prop defined.
     For example, If you are using a 3rd-party custom-input component that requires a `data-tooltip` attribute on the input then you can add this attribute to component instance,
     ```javascript
     <custom-input data-tooltip="Enter your input" />
     ```
     If you try to pass the props from parent component the child props with the same names will be overridden. But props like `class` and `style` are exception to this, these values will be merged in the child component.
     ```javascript
     //Child component
     <input type="date" class="date-control">
     //Parent component
     <custom-input class="custom-class" />
     ```
38.  ### Describe about validations available for props?
     Vue provides validations such as type, required fields, default values along with customized validations. You can provide an object with validation requirements to the value of props as below,
     Let's take an example of user profile Vue component with possible validations,
     ```javascript
     Vue.component('user-profile', {
       props: {
         // Basic type check (`null` matches any type)
         age: Number,
         // Multiple possible types
         identityNumber: [String, Number],
         // Required string
         email: {
           type: String,
           required: true
         },
         // Number with a default value
         minBalance: {
           type: Number,
           default: 10000
         },
         // Object with a default value
         message: {
           type: Object,
           // Object or array defaults must be returned from
           // a factory function
           default: function () {
             return { message: 'Welcome to Vue' }
           }
         },
         // Custom validator function
         location: {
           validator: function (value) {
             // The value must match one of these strings
             return ['India', 'Singapore', 'Australia'].indexOf(value) !== -1
           }
         }
       }
     })
     ```
39.  ### How do you customize model directive for a component?
     The v-model directive on a component uses **value** as the prop and **input** as the event, but some input types such as `checkboxes` and `radio buttons` may need to use the value attribute for a server side value. In this case, it is preferred to customize model directive. Let's take an example of checkbox component,
     ```javascript
     Vue.component('custom-checkbox', {
       model: {
         prop: 'checked',
         event: 'change'
       },
       props: {
         checked: Boolean
       },
       template: `
         <input
           type="checkbox"
           v-bind:checked="checked"
           v-on:change="$emit('change', $event.target.checked)"
         >
       `
     })
     ```
     Now you can use v-model on this customized component as below,
     ```javascript
     <custom-checkbox v-model="selectFramework"></custom-checkbox>
     ```
     The selectFramework property will be passed to the checked prop and same property will be updated when custom checkbox component emits a change event with a new value.
40.  ### What are the possible ways to provide transitions?
     There are many ways Vue provides transition effects when items are inserted, updated, or removed from the DOM. Below are the possible ways,
     1. Automatically apply classes for CSS transitions and animations
     2. Integrate 3rd-party CSS animation libraries. For example, Animate.css
     3. Use JavaScript to directly manipulate the DOM during transition hooks
     4. Integrate 3rd-party JavaScript animation libraries. For example, Velocity.js
41.  ### What is vue router and their features?
     Vue Router is a official routing library for single-page applications designed for use with the Vue.js framework. Below are their features,
     1. Nested route/view mapping
     2. Modular, component-based router configuration
     3. Route params, query, wildcards
     4. View transition effects powered by Vue.js' transition system
     5. Fine-grained navigation control
     6. Links with automatic active CSS classes
     7. HTML5 history mode or hash mode, with auto-fallback in IE9
     8. Restore scroll position when going back in history mode

42.  ### What are the steps to use vue router and give an example?
     It is easy to integrate vue router in the vue application. Let us see the example with step by step instructions.
     **Step 1:** Configure router link and router view in the template
     ```javascript
     <script src="https://unpkg.com/vue/dist/vue.js"></script>
     <script src="https://unpkg.com/vue-router/dist/vue-router.js"></script>

     <div id="app">
       <h1>Welcome to Vue routing app!</h1>
       <p>
         <!-- use router-link component for navigation using `to` prop. It rendered as an `<a>` tag -->
         <router-link to="/home">Home</router-link>
         <router-link to="/services">Services</router-link>
       </p>
       <!-- route outlet in which component matched by the route will render here -->
       <router-view></router-view>
     </div>
     ```
     **Step 2:** Import Vue and VueRouter packages and then apply router
     ```javascript
     import Vue from 'vue';
     import VueRouter from 'vue-router';

     Vue.use(VueRouter)
     ```
     **Step 3:** Define or import route components.
     ```javacript
     const Home = { template: '<div>Home</div>' }
     const Services = { template: '<div>Services</div>' }
     ```
     **Step 4:** Define your route where each one maps to a component
     ```javascript
     const routes = [
       { path: '/home', component: Home },
       { path: '/services', component: Services }
     ]
     ```
     **Step 5:** Create the router instance and pass the `routes` option
     ```javascript
     const router = new VueRouter({
       routes // short for `routes: routes`
     })
     ```
     **Step 6:**  Create and mount the root instance.
     ```javacript
     const app = new Vue({
       router
     }).$mount('#app')
     ```

     Now you are able to navigate different pages(Home, Services) with in Vue application.
43.  ### What is dynamic route matching?
     Sometimes it may be required to map routes to the same component based on a pattern. Let's take a user component with the mapped URLs like `/user/john/post/123` and `/user/jack/post/235` using dynamic segments,
     ```javascript
     const User = {
       template: '<div>User {{ $route.params.name }}, PostId: {{ route.params.postid }}</div>'
     }

     const router = new VueRouter({
       routes: [
         // dynamic segments start with a colon
         { path: '/user/:name/post/:postid', component: User }
       ]
     })
     ```
44.  ### How to make router param changes as reactive?
     When you navigate from one URL to other(mapped with a single component) using routes with params then the same component instance will be reused. Even though it is more efficient than destroying the old instance and then creating a new one, the lifecycle hooks of the component will not be called. This problem can be solved using either of the below approaches,
     1. Watch the $route object:
     ```javascript
     const User = {
       template: '<div>User {{ $route.params.name }} </div>',
       watch: {
         '$route' (to, from) {
           // react to route changes...
         }
       }
     }
     ```
     2. Use beforeRouteUpdate navigation guard: This is only available in 2.2 version.
     ```javascript
     const User = {
       template: '<div>User {{ $route.params.name }} </div>',
       beforeRouteUpdate (to, from, next) {
         // react to route changes and then call next()
       }
     }
     ```
45.  ### What is route matching priority?
     Sometimes the URL might be matched by multiple routes and the confusion of which route need to be mapped is resolved by route matching priority. The priority is based on order of routes configuration. i.e, The route which declared first has higher priority.
     ```javascript
     const router = new VueRouter({
            routes: [
              // dynamic segments start with a colon
              { path: '/user/:name', component: User } // This route gets higher priority
              { path: '/user/:name', component: Admin }
              { path: '/user/:name', component: Customer }
            ]
          })
     ```
46.  ### What are nested routes?
     Generally, the app is composed of nested components which are nested multiple levels deep. The segments of a URL corresponds to a certain structure of these nested components. To render components into the nested outlet, you need to use the `children` option in `VueRouter` constructor config.
     Let's take a user app composed of profile and posts nested components with respective routes. You can also define a default route configuration when there is no matching nested route.
     ```javascript
     const router = new VueRouter({
       routes: [
         { path: '/user/:id', component: User,
           children: [
             {
               // UserProfile will be rendered inside User's <router-view> when /user/:id/profile is matched
               path: 'profile',
               component: UserProfile
             },
             {
               // UserPosts will be rendered inside User's <router-view> when /user/:id/posts is matched
               path: 'posts',
               component: UserPosts
             },
               // UserHome will be rendered inside User's <router-view> when /user/:id is matched
             {  path: '',
                component: UserHome },
           ]
         }
       ]
     })
     ```
47.  ### What are single file components?
     Single File Components are an easy concept to understand. Earlier you might heard about all three parts(HTML, JavaScript and CSS) of your application kept in different components. But Single File Components encapsulate the structure, styling and behaviour into one file. In the beginning, it seems strange to have all three parts in one file, but it actually makes a lot more sense.
     Let's take an example of Singile File Components
     ```javascript
     <template>
         <div>
             <h1>Welcome {{ name }}!</h1>
         </div>
     </template>

     <script>
         module.exports = {
            data: function() {
                return {
                    name: 'John'
                }
            }
         }
     </script>

     <style scoped>
         h1 {
             color: #34c779;
             padding: 3px;
         }
     </style>
     ```
48.  ### Is Single File Components violating separation of concerns?
     As per the latest modern UI development, separation of concerns is not equal to separation of file types. So it is preferred to divide codebase layers into loosely-coupled components and compose them instead of dividing the codebase into three huge layers that interweave with one another. This way it makes Single File Components more cohesive and maintainable by combining template, logic and styles together inside a component.
     You can also still maintain javascript and CSS files as separate with hot-reloading and pre-compilation features. For example,
     ```
     <template>
       <div>This section will be pre-compiled and hot reloaded</div>
     </template>
     <script src="./my-component.js"></script>
     <style src="./my-component.css"></style>
     ```
49.  ### What are the problems solved by Single File Components?
     The Single File Components solve the common problems occurred in a javascript driven application with a .vue extension. The list of issues are,
     1. Global definitions force unique names for every component
     2. String templates lack syntax highlighting and require ugly slashes for multiline HTML
     3. No CSS support means that while HTML and JavaScript are modularized into components, CSS is conspicuously left out
     4. No build step restricts us to HTML and ES5 JavaScript, rather than preprocessors like Pug (formerly Jade) and Babel
50.  ### What are filters?
     Filters can be used to apply common text formatting. These Filters should be appended to the end of the JavaScript expression, denoted by the “pipe” symbol. You can use them in two specific cases:
     1. mustache interpolations
     2. v-bind expressions

     For example, Let's define local filter named camelcase in a component’s options
     ```javascript
     filters: {
       capitalize: function (value) {
         if (!value) return ''
         value = value.toString()
         return value.charAt(0).toUpperCase() + value.slice(1)
       }
     }
     ```
     Now you can use the filter in either mustache interpolation or v-bind expression,
     ```javascript
     <!-- in mustaches -->
     {{ username | camelcase }}

     <!-- in v-bind -->
     <div v-bind:id="username | capitalize"></div>
     ```
51.  ### What are the different ways to create filters?
     You can define filters in two ways,
     1. **Local filters:**
     You can define local filters in a component’s options. In this case, filter is applicable to that specific component.
     ```javascript
     filters: {
       capitalize: function (value) {
         if (!value) return ''
         value = value.toString()
         return value.charAt(0).toUpperCase() + value.slice(1)
       }
     }
     ```
     2. **Global filters:**
     You can also define a filter globally before creating the Vue instance. In this case, filter is applicable to all the components with in the vue instance,
     ```javascript
     Vue.filter('capitalize', function (value) {
       if (!value) return ''
       value = value.toString()
       return value.charAt(0).toUpperCase() + value.slice(1)
     })

     new Vue({
       // ...
     })
     ```
52.  ### How do you chain filters?
     You can chain filters one after the other to perform multiple manipulations on the expression. The generic structure of filter chain would be as below,
     ```javascript
     {{ message | filterA | filterB | filterB ...}}
     ```
     In the above chain stack, you can observe that message expression applied with three filters, each separated by a pipe(|) symbol. The first filter(filterA) takes the expression as a single argument and the result of the expression becomes an argument for second filter(filterB) and the chain continue for remaining filters.
     For example, if you want to transform date expression with a full date format and uppercase then you can apply dateFormat and uppercase filters as below,
     ```javascirpt
     {{ birthday | dateFormat | uppercase}}
     ```

53.  ### Is it possible to pass parameters for filters?
     Yes, you can pass arguments for a filter similar to a javascript function. The generic structure of filter parameters would be as follows,
     ```javascript
     {{ message | filterA('arg1', arg2) }}
     ```
     In this case, filterA takes message expression as first argument and the explicit parameters mentioned in the filter as second and third arguments.
     For example, you can find the exponential strength of a particular value
     ```javascript
     {{ 2 | exponentialStrength(10) }} // prints 2 power 10 = 1024
     ```
54.  ### What are plugins and their various services?

     Plugins provides global-level functionality to Vue application. The plugins provides various services,
     1. Add some global methods or properties. For example, vue-custom-element
     2. Add one or more global assets (directives, filters and transitions). For example, vue-touch
     3. Add some component options by global mixin. For example, vue-router
     4. Add some Vue instance methods by attaching them to Vue.prototype.
     5. A library that provides an API of its own, while at the same time injecting some combination of the above. For example, vue-router
55.  ### How to create a plugin?
     The Plugin is created by exposing an install method which takes Vue constructor as a first argument along with options. The structure of VueJS plugin with possible functionality would be as follows,
      ```javascript
      MyPlugin.install = function (Vue, options) {
        // 1. add global method or property
        Vue.myGlobalMethod = function () {
          // some logic ...
        }

        // 2. add a global asset
        Vue.directive('my-directive', {
          bind (el, binding, vnode, oldVnode) {
            // some logic ...
          }
          ...
        })

        // 3. inject some component options
        Vue.mixin({
          created: function () {
            // some logic ...
          }
          ...
        })

        // 4. add an instance method
        Vue.prototype.$myMethod = function (methodOptions) {
          // some logic ...
        }
      }
      ```
56.  ### How to use a plugin?
     You can use plugin by passing your plugin to Vue's **use** global method. You need to apply this method before start your app by calling new Vue().
     ```javascript
     // calls `MyPlugin.install(Vue, { someOption: true })`
     Vue.use(MyPlugin)

     new Vue({
       //... options
     })
     ```