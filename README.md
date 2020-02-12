Q1: Is the keyword "fixes" the only way to auto-close an issue from a PR 
(pull request). Is there other keywords that can accomplish the same thing?

As: there are a list to do for pulling requests:
close
closes
closed
fix
fixes
fixed
resolve
resolves
resolved

Q2: Do you have to create a new PR EVERYTIME you want to close an issue,
or is it possible to close multiple issues within a single PR? If so, 
how?
As: You can ise coma to close mutliple pull requests. Ex. Closes #1, #2, #3

Q3: Provide an example of using map that is different from the one I have done.
Your example must use map both as a named function declaration and with an
anonymous function. 

Within comments, explain exactly what map is doing. Finally, why is the
"transformation function" we discussed in class sometimes referred to 
as a callback function. 

As: 
<!-- A transformation function or callback is a function that is to be executed after another function has finished executing — hence the name ‘call back’.-->
1st case:
    function changeNumber(number){
    return number -1
}

var value=['1', '2', '3'].map(changeNumber);
console.log(value)


['1', '2', '3'].map(function changeNumber(number)); 
<!-- input: [1,2,3] -->
<!-- call the inner function to map the original list for each element reducing one -->
<!-- output: [0,1,2] -->


var numbers = [1, 2, 3];
var triples = numbers.map(function(num) {
  return num ** 3;
});
<!-- input: [1,2,3] -->
<!-- make a function with the formula with number power of three to return the value-->
<!-- output: [1,8,27] -->
