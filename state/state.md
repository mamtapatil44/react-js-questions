# state:
# - To manage data inside the react componant we use state
# -  If we wamt dynamically chnage the value of any variable then use state and useState hook.
# - with normal variable ,react not allow to update value in Dom, it cant rerender the component.But we use state variaable,it will rerender our component and value will refflect on ui as it it updated in DOM.
# state works asynchrounously so we cant use it it if condition or loop fo riteration.
# to use state we have to import useState()  hook form react lib , which is named import 
# we can pass default value in useState("") hook ,which returns array of[ variableName ,setVariable] = useState("");
# here varaible  name is which varaible we have to update and 2nd one is dispatch action,means method to update that state
# we can update object with previousobct and spead operator
# for array updation we use map for iteration and for certion object we use condtion and after that use use dispactcher with spread poerator and new value


# What is the difference between useState and useReducer?
 # Use useState for simple state updates and useReducer for more complex logic, especially when state transitions depend on previous state.
 # useState():::::
 <!-- # const [count, setCount] = useState(0);
 # setCount(count + 1); -->
 
 # useReducer():::::::
 <!-- const reducer = (state, action) => {
  switch (action.type) {
    case "increment":
      return { count: state.count + 1 };
    case "decrement":
      return { count: state.count - 1 };
    default:
      return state;
  }
};

const [state, dispatch] = useReducer(reducer, { count: 0 });
dispatch({ type: "increment" }); -->




# 10. How do I share state between components?
# 1 Passing state as props