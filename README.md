
# JavaScript DOM & Events – Q&A (Module 25, Milestone 4)

## 1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

- **getElementById()** → Selects one element by `id`. Returns a single element.
- **getElementsByClassName()** → Selects elements by class name. Returns a live HTMLCollection.
- **querySelector()** → Returns the first element matching a CSS selector.
- **querySelectorAll()** → Returns all elements matching a CSS selector (static NodeList).

---

## 2. How do you create and insert a new element into the DOM?

```javascript
const div = document.createElement("div");
div.innerText = "Hello World";
document.body.appendChild(div);
```

Steps:
1. Create the element  
2. Add content  
3. Insert into the DOM  

---

## 3. What is Event Bubbling? And how does it work?

Event Bubbling is a process where an event starts from the target element and moves upward to its parent elements.

Example: Clicking a button inside a div triggers the button event first, then the parent div event.

---

## 4. What is Event Delegation in JavaScript? Why is it useful?

Event Delegation is attaching a single event listener to a parent element to handle events for its child elements.

It is useful because:
- Improves performance  
- Works for dynamically added elements  
- Reduces multiple event listeners  

---

## 5. What is the difference between preventDefault() and stopPropagation() methods?

- **preventDefault()** → Prevents the browser’s default behavior (e.g., form submission).
- **stopPropagation()** → Stops the event from bubbling to parent elements.