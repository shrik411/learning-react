# learning-react
1. React Hooks 
*  useState
   let [count, setCount] = useState(0)
   
* useEffect
  useEffect hook can replace functionality of componentDidMount, componentDidUnmount and ComponentDidUpdate 
useEffect(() => {
  // code snippet here
}, [<dependancies>]);

* useContenxt
context is use for passing the property down to the child components in nested hierarchy
        A  {context} 
B       C       D 
E       F       G 
                H { needed here } 
                
Class Component
export const userContext = React.createContext()
export const channelContext = React.createContext()

<userContext.Provider value={'name'}> 

   <channelContext.Provider value={'contextValue'}>
   
      <Component C/>
      
   </channelContext.Provider>
   
<userContext.Provider

