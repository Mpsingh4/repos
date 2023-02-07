### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.


``` javascript
 const whatToDoForLunch = function(hungry, availableTime) {

  if (hungry === true && availableTime < 20) {
    console.log("Pick up a snack or grab something you already have at home!");
  } else if (hungry === true && (availableTime <= 30 && availableTime > 20)) {
    console.log("you deserve a break and should take time to cook a tasty meal");
  } else if (hungry === true && availableTime > 30) {
    console.log("this is a pretty intense program, reconsider");
  } else if (hungry === false) {
    console.log("keep on coding");
  }

  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
};

console.log(whatToDoForLunch(false, 35));
```