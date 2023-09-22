• Explain Life cycle in Class Component and functional component with Hooks.
ANS:-
A React component undergoes three different phases in its lifecycle,
Including mounting , updating , and unmounting. Each PHASE HAS SPECIFIC METHODS RESPONSIBLE FOR A PARTICULAR STAGE IN A COMP0NENT’S LIFECYCLE. 
React lifecycle methods
 
PHASES OF A REACT COMPONENT’S LIFECYCLE
A REACT COMPONENT UNDERGOES THREE PHASES IN ITS LIFECYCLE. Mounting, updating and unmounting. 
1.	1 The mounting phase is when a new component is created and inserted into the DOM or, in other words, when the life of a component begins. This can only happen once, and is often called “initial render.”
2.	The updating phase is when the component updates or re-renders. This reaction is triggered when the props are updated or when the state is updated. This phase can occur multiple times, which is kind of the point of React.
3.	The last phase within a component's lifecycle is the unmounting phase, when the component is removed from the DOM.
In a class-based component, you can call different methods for each phase of the lifecycle (more on this below). These lifecycle methods are of course not applicable to functional components because they can only be written/contained within a class. However, React hooks give functional components the ability to use states.
Hooks have gaining popularity because they make working with React cleaner and often less verbose.
The mounting phase
In the mounting phase, a component is prepared for and actually inserted into the DOM. To get through this phase, four lifecycle methods are called: constructor, static getDerivedStateFromProps, render, and componentDidMount.

The updating phase
The Updating phase is triggered when component props or state change, and consists of the following methods: static getDerivedFromProps, shouldComponentUpdate, render, getSnapshotBeforeUpdate, and componentDidUpdate. The methods getDerivedFromProps and render are also part of the mounting phase. Since they’ve been covered previously, this section focuses on the other three methods.

The unmounting phase
The unmounting phase is the third and final phase of a React component. At this phase, the component is removed from the DOM. Unmounting only has one lifecycle method involved: componentWillUnmount.

React Hooks and the component lifecycle
Versions of React before 16.8 consider two kinds of components based on statefulness: the class-based stateful component, and the stateless functional components (often referred to as a “dumb component”). But with the release of React 16.8, Hooks were introduced and empowered developers to access state from functional components, instead of writing an entire class. With this change, building components became easier and less verbose.
Hooks known as default hooks come with React, and you’re also able to create your own custom hook. A custom hook is just a function that starts with use, like “useStore, or useWhatever.”
The two most common default hooks are useState and useEffect. The useState hook gives state to the functional component, and useEffect allows you to add side effects within it (like after initial render), which aren’t allowed within the function's main body. You can also act upon updates on the state with useEffect.
React has released more default hooks, but useState and useEffect are the ones you should be most familiar with. Let’s take a look at how they work and compare them to the component lifecycle we covered above.
REACT Hooks list
useState
useEffect
useContext
useLayoutEffect
useReducer
useCallback
useMemo
useRef
useTransition
useDeferredValue
useId

