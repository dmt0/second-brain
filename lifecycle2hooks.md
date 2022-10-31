```javascript
componentWillMount()

export const useComponentWillMount = (callback) => {
  const willMount = useRef(true);
  if (willMount.current) {
    callback();
  }
  willMount.current = false;
};


componentDidMount()

useEffect(() => {
  // Your code here
}, []);


componentDidMount() + componentWillUnmount()

useEffect(() => {
  Subscribe()
  return () => {
    Unsubscribe()
  }
}, [])


UNSAFE_componentWillReceiveProps()

useEffect( () => {
   ...
}, [someProps])


componentDidUpdate()

useEffect( () => {
  // Your code here
})
