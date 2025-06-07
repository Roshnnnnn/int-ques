# int-ques
interview questions of HTML CSS Javascript react and typescript
# 🧠 Full Stack Interview Questions (React, JavaScript, TypeScript, HTML, CSS)

---

## 🔷 React Questions
1. What is the difference between functional and class components?
Ans=
## 1. ✅ Functional Component (React v18 ke baad recommended)
Ye ek plain JavaScript function ki tarah likha jata hai.

Shorter, cleaner, and easy to read.

React v16.8 ke baad isme Hooks ka use shuru hua (like useState, useEffect).

Mostly modern React apps isi ka use karti hain.

function Hello() {
  return <h1>Hello Functional Component</h1>;
}


## 2. 🧱 Class Component (Old Approach)
Ye ek JavaScript class hoti hai jo React.Component ko extend karti hai.

Code thoda lamba aur complex hota hai (boilerplate code).

Isme lifecycle methods use hote hain jaise componentDidMount, componentWillUnmount, etc.

this.state aur this.setState() se state manage hoti hai.

class Hello extends React.Component {
  constructor(props) {
    super(props);
    this.state = { message: "Hello Class Component" };
  }

  render() {
    return <h1>{this.state.message}</h1>;
  }
}

2. How does useState work?
## Ans= useState ek tarike ka hook h jo v18 main use hota h. Isme values jo h hum store krte h chahe wo jo b ho object, array, string kuch b wo store kr leta h.

4. What is useEffect and when should you use it?
## Ans= useEffect hook h react main jo functional component main use krte h ye ek tarike ka side effect kohandle krte h isme call back hota h or isme dependency array hota h iske andr hum api call krwa skte h settimeout use kr skte h setinterval use kr skte h, dom manupilate kr skte h, localStorage ko use krte h, page title change krta h.

5. What are props and how do they differ from state?
## Ans= State:- 
## 1. iske andr value ko store kr skte h 
## 2. ye mutable kr skte h
## Props:- 
## 1. iske andr value ko store kr skte h 
## 2. ye mutable nahi kr skte h
## 3. ye parent to child move hota h 
## 4. ye readable hota h 

6. What is JSX?
## Ans:- It is a combination of JavaScript and Xml, in react you can write JS and HTML combine.

7. How do you handle forms in React?
## Ans:- 1.  useState main value store krna.
## 2. onchange 
## 3. onSubmit

8. How can you lift state up in React?
## Ans:- jb kbhi 2 different prop ko same data chahiye to unke parent component main daal kr dono props ko bheja jae usse lifting up state kehte h.

9. What is the virtual DOM?
## Ans= ye ek real doe ki replica hoti h jo real dom main changes hone se phele check krta h ki changes kon se node main hua h fir sirf ussi change ko update krta h real dom main

10. What are controlled vs uncontrolled components?
## Ans= controlled:- isme state main value store hoti h, onchange pr access hota h, jldi update krta h 

## unControlled:- ye direct dom handle krta h, ref access krta h, limited controll hota h 

11. What is the purpose of keys in a list?
## Ans:- keys ka use hum isiliye krte h kyuki jb b hum chize update, delete, edit krte h to chize proper ho id's pr.

12. How do you pass data from child to parent?
## Ans= waise react main data unidirectional main flow krta h but agar koi jruri h to isse callback ki help se child to parent main bhej skte ho

13. What is React Router and how do you implement routing?
## Ans:- single page applications main hum direct page navigate ni kr skte h to react routing do ko npm krte h or ye ek page se dusre page pr redirect krta h home se contact or contact se other page pr 

14. What are custom hooks?
## Ans- Custom hooks wo hooks h wo hum apne hisab se bnate h like koi b logi baar baar call krwana hota h to hr page pr bnane se btr ek alag jgh bna do or jha use krna h wha get kro

15. How do you fetch data in React (API calls)?
## Ans- Axios, fetch, promises in sbhi ko hum useEffect main call krwa skte h.

16. What is React.memo and when should you use it?
## Ans- React.memo ye memoized krta h component ko, ye ek higher order component hota h jo tb hi re render hota h jb changes hote h.

17. What is useCallback vs useMemo?
## Ans- useMemo:- return krta h value, remember krta h value, avoid krta h big calculation ko krne pr 
## useCallback:- return krta h function, remember krta h function, avoid krta h kisi component ko baar baar create krne se 

18. What is Context API? Compare with Redux.
## Ans:- Context API:- Light weight, state update through useState & reducer ka use krte h, 
## Redux:- heavy bundle, big project main use krte h, middleware hote h, 

19. How does reconciliation work in React?
## Ans:- reconciliation means check krna changes kha kha hua h kon se node main 

20. What is forwardRef and why use it?
## Ans= 

21. How to lazy load components in React?
## Ans:- lazy laoding ka use hum isiliye krte h taki component ko tbhi load kiya jaa ske jb iski jrurt ho.

22. What are error boundaries?
## Ans- iska use tb kiya jata h taki child component main koi error aae to uss se bacha ske, crash hone se bachata h, ek fallback UI dikhata h

23. What is hydration in React SSR?
## Ans- 

24. How do you avoid unnecessary re-renders?
## Ans- memo, useMemo, callback, code splitting, kisi b state ko unnecessary update krna.

25. How do you optimize performance in large React apps?
## Ans- memo, useMemo, callback, lazy loading, debounce, image optimization.

26. How do you test React components?
## Ans- jest, react testing library se inko npm kro or fir 
## kyu krte h :- check krne k liye UI ka behviour, bugs check krne k liye

---

## 🟨 JavaScript Questions
1. What are let, const, and var?
## Ans:- var:- isko hum re declare kr skte h, value re assign kr skte h, 
## let:- block scope, hum re declare ni kr skte h, value re assign kr skte h, 
## const:- block scope, hum re declare ni kr skte h, value re assign ni kr skte h, 

2. What is hoisting?
## Ans:- kisi b value ko assign krne se pehle call krna ko hoisting kehte h 

3. Difference between == and ===?
## Ans- === data, value type check krta h
## == value check krta h 

4. What is a closure?
## Ans- jb kisi function k andr kisi function ko likha jae or jo inner wala function h na wo parent function k andr ki value ko access kr ske usse closure kehte h.

5. What is the `this` keyword?
## Ans- js main `this` ek keyword h jiska kaam hota h apne current object ya parent context ko reffer krna.

6. What are promises and how does async/await work?
## Ans- js sync work krta h but kuch chizo k liye async kaam krwana pdta h to promises or async await ka use krna pdta h promises main 3 stage hote h pending, fullfilled, rejected. async/await main same work krta h promises ka updated version keh skte h.

7. What is a callback function?
## Ans- function k andr ek dusra function call krwana or jo baad main chlta h usse callback function kehte h 

8. What is event bubbling and how do you prevent it?
## Ans- jb kbhi div k andr multiple div ho or sbse andr wale div pr click krne pr bhaar k div b activate ho jae ya click ho jae use event bubbling kehte h isko rokne k liye stop propogation() ka use krte h 

9. What is destructuring?
## Ans- iska mtlb kisi object, array main multiple data ho usse unpack krna usse destructure kehte h 

10. What is the spread/rest operator?
## Ans- rest- isme jo unpack hua h variable usse wapas pack krna.
## spread- isme packed ko unpack krna variables ko

11. What are higher-order functions?
## Ans- ek function k andr dusre function ko as a argument lena or whi function return krna hof kehlata h 

12. How does the event loop work (call stack, microtasks, macrotasks)?
## Ans- 

13. What are generators?
## Ans- 

14. Explain memory management and garbage collection.
15. Difference between deep copy and shallow copy.
16. What is prototypal inheritance?
17. How do ES6 modules differ from older module patterns?
18. What is throttling vs debouncing?
19. What are WeakMap and WeakSet?
20. What is currying in JavaScript?
21. What is tail call optimization?

---

## 🟦 TypeScript Questions
1. What is TypeScript and how is it different from JavaScript?
2. What are interfaces and types in TypeScript?
3. What is the difference between interface and type?
4. What is type inference?
5. How do you define optional and readonly properties?
6. How do you define a function with typed parameters and return type?
7. What is a union type? What is an intersection type?
8. What is `any`, `unknown`, `never`, and `void`?
9. What are generics and how do you use them?
10. How does TypeScript handle enums?
11. How do you extend interfaces?
12. How do you use TypeScript with React (props and state)?
13. What is type assertion in TypeScript?
14. How do you handle third-party JavaScript libraries in TypeScript?
15. What is a utility type in TypeScript (e.g., Partial, Pick, Omit)?
16. How do modules and namespaces differ in TypeScript?
17. What are declaration files (`.d.ts`)?
18. How does TypeScript support strict type checking?
19. What is structural typing in TypeScript?
20. What is the use of `keyof`, `typeof`, and `in`?

---

## 🟩 HTML Questions
1. Difference between `<div>` and `<span>`?
2. What are semantic HTML elements?
3. Difference between `id` and `class`?
4. How do forms work in HTML?
5. How to embed images, videos, and audios?
6. What are meta tags?
7. What is the difference between `<section>`, `<article>`, and `<aside>`?
8. How to create hyperlinks and buttons?
9. What is the `alt` attribute used for?
10. What are self-closing tags?
11. How do you make a website accessible (ARIA)?
12. Difference between `defer` and `async` for scripts?
13. What is the Shadow DOM?
14. What are Web Components?
15. Benefits of HTML5 over previous versions?

---

## 🟧 CSS Questions
1. Difference between `id` and `class` selectors?
2. What is the CSS box model?
3. How to center a div (horizontal and vertical)?
4. Explain `position: relative`, `absolute`, `fixed`, and `sticky`.
5. What are Flexbox and Grid? When to use which?
6. Difference between em, rem, %, px, vw, and vh?
7. What is specificity in CSS?
8. How do pseudo-classes and pseudo-elements work?
9. What is z-index and how does stacking context work?
10. What are CSS variables?
11. What is the BEM naming convention?
12. How do you create a responsive design?
13. How to build responsive UI without media queries?
14. What are transitions and animations in CSS?
15. What does `will-change` do and how does it improve performance?
16. What are utility-first frameworks like Tailwind CSS?
17. How do you implement dark/light themes with CSS?

