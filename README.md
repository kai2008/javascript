# javascript


# callback function example

```
function createQuote(quote, callback){ 
  var myQuote = "Like I always say, " + quote;
  callback(myQuote); // 2
}

createQuote("eat your vegetables!", function(q){ 
  console.log(q); 
});


createQuote("eat your vegetables!", printNewQuote);

function printNewQuote(q) {
	console.log(q);
}
```

# callback function with 2 arguments
```
function createQuote(quote, callback){ 
  var myQuote = "Like I always say, " + quote;
  callback(myQuote); // 2
}

// anonymous function callback
createQuote("eat your vegetables!", function(q,p){ 
  console.log(q,p); 
});


function printNewQuote(q, p) {
	console.log(q,p);
}

createQuote("eat your vegetables!", printNewQuote);
```

# test on https://jsconsole.com/

# reference
* https://forum.freecodecamp.org/t/javascript-callback-functions-explained-how-to-use-callbacks-in-javascript/14658
