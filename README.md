# EloquentNotes
Eloquent Javascript Notes
Exercise on Recursion
//This program takes a number and provides true if number even else false if odd.
function isEven(n) {
  //if 0 then must be even
  if (n == 0) return true;
  //if 1 will be false
  else if (n == 1) return false;
  // if the number is less than 0 then negative value
  else if (n < 0) return isEven(-n);
  // -2 to value if or 0, this is the recursive function.
  else return isEven(n - 2);
}

console.log(isEven(50));
// → true
console.log(isEven(75));
// → false
console.log(isEven(-1));
// → false
__________________________________________________________________________________________________________________________________________________________________

