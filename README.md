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

# test on https://jsconsole.com/
