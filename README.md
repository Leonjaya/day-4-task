# day-4-task
(function(arr) {
console.log(arr.filter(num => num % 2 !== 0));
})([1, 2, 3, 4, 5, 6, 7, 8, 9]);

@Leonjaya
Owner
Author
Leonjaya commented on 325ef97 last week
(function(arr) {
console.log(arr.map(str => str.charAt(0).toUpperCase() + str.slice(1).toLowerCase()));
})(["hello", "world", "javascript"]);

@Leonjaya
Owner
Author
Leonjaya commented on 325ef97 last week
(function(arr) {
console.log(arr.reduce((sum, num) => sum + num, 0));
})([1, 2, 3, 4, 5]);

@Leonjaya
Owner
Author
Leonjaya commented on 325ef97 last week
(function(arr) {
const isPrime = num => {
if (num <= 1) return false;
for (let i = 2; i < num; i++) {
if (num % i === 0) return false;
}
return true;
};
console.log(arr.filter(isPrime));
})([1, 2, 3, 4, 5, 6, 7, 8, 9]);

@Leonjaya
Owner
Author
Leonjaya commented on 325ef97 last week
(function(arr) {
const isPalindrome = str => str === str.split('').reverse().join('');
console.log(arr.filter(isPalindrome));
})(["madam", "racecar", "hello", "world"]);

@Leonjaya
Owner
Author
Leonjaya commented on 325ef97 last week
(function(arr1, arr2) {
const mergeArrays = (a, b) => a.concat(b).sort((x, y) => x - y);
const findMedian = arr => {
const mid = Math.floor(arr.length / 2);
return arr.length % 2 !== 0 ? arr[mid] : (arr[mid - 1] + arr[mid]) / 2;
};
const mergedArray = mergeArrays(arr1, arr2);
console.log(findMedian(mergedArray));
})([1, 3, 5], [2, 4, 6]);

@Leonjaya
Owner
Author
Leonjaya commented on 325ef97 last week
(function(arr) {
console.log([...new Set(arr)]);
})([1, 2, 2, 3, 4, 4, 5]);

@Leonjaya
Owner
Author
Leonjaya commented on 325ef97 last week
(function(arr, k) {
const rotateArray = (a, k) => {
k = k % a.length;
return a.slice(-k).concat(a.slice(0, -k));
};
console.log(rotateArray(arr, k));
})([1, 2, 3, 4, 5], 2);
