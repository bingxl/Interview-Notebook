

64.js代码,使用尾调用优化, 不存在函数调用栈过长问题
```javascript
function sumSolution(n, sum=1) {
  if(!n) {
    return sum;
  } 
  return sumSolution(n - 1, sum * n);
}
```
