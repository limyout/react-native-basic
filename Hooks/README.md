
## React hooks(UseEffect) 사용하기
<br>

**rendering**
"Rendering" refers to the constant task of converting data into html and transferring it to the renderer
<br>
<br>

**useEffect**
* It is useEffect that allows the functions to be used at once when componentDidMount, componentDidUpdate, and componentWillUnmount is active.
* UseEffect runs after the Dom is updated or the state is changed.
<br>
<br>

**Dom?** ; Document Object Model
<br>
* A method of expressing structured documents through objects, written in HTML.
* Web browsers use DOM to apply javascript and CSS to objects.
<br>
<br>

**Hooks rule?**
<br>

1. It must be written at the top of the react function.
- Do not use within conditional statements, internal functions, or repeating statements.

2. Use only within the react function.
- Exceptional call within the custom function
<br>

ex)
```
const [name, setName] = useState("");

useEffect(()=>{

document.title = `search search search my ${name}`;

});
```
<br>
