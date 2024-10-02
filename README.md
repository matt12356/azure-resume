# azure-resume
the resume i built using the Azure cloud resume challenge as inspiration

## The Begining 

-frontend folder contains the webpage.

-main.js contains visitor counter code. example below 

```js
window.addEventListener('DOMContentLoaded', (event) =>{
    getVisitCount();
})

const functionAPI = '';

const getVisitCount = () => {
    let count = 30;
    fetch(functionAPI).then(response => {
        return response.json()
    }).then(response =>{
        console.log("website called function API");
        count = response.count;
        document.getElementById("counter").innerText = count;
    }).catch(function(error){
        console.log(error);
    });
    return count;
}
```
 



