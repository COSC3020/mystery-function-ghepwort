# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

This function finds the largest value in an array. It works by breaking the array into smaller and smaller arrays recursivly by excluding the first value. This goes until there is an array with an array length of 1 (the base case). The algorithm then goes up and compares the first values in the array of length 1 and 2 to see which one is larger. Whichever one is larger then is returned and then compared against the first value of length 3. The larger is returned and this process is repeated till you get to the original array and whatever value is larger at the end is returned giving us the largest value in the array.


I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.