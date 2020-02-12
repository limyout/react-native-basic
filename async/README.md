## AsyncStorage


* Using Promise

```
const makeGetRequest = () =>
 getJSON().then(response => {
 console.log(response); // this will log JSON data
 return "done";
});
 
makeGetRequest();
```

 

* Using async/await

```
const makeGetRequest = async () => {
 console.log(await getJSON()); // this will log response/JSON data
 return "done";
};
 
makeGetRequest();
```
