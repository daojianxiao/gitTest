# gitTest
:memo: Web 前端学习笔记
# 作业
### 1) 补全下面的函数
``` // 对 a 和 b 做加法
    function add(a, b) {
      // 你写的内容
    }
    
    add(1, 2) // 返回值 3
    add(1, -2) // 返回值 -1
```
#### 答案
```
function add(a, b) {
      return a+b;
    } 
    add(1, 2) // 返回值 3
    add(1, -2) // 返回值 -1
```
### 2) 补全下面的函数
```
 function shouldWork(date) {
      // 你写的内容。分别实现用 if 和 switch 实现。
    }

    shouldWork('周一') // 返回值是 上班
    shouldWork('周二') // 返回值是 上班
    shouldWork('周三') // 返回值是 上班
    shouldWork('周四') // 返回值是 上班
    shouldWork('周五') // 返回值是 上班
    shouldWork('周六') // 返回值是 上班
    shouldWork('周日') // 返回值是 上班
```
#### 答案
```
1、function shouldWork(date) {
      var x="";
var week=new Date().getDay();
if(week<7){
x="上班";
}
document.getElementById("demo").innerHTML=x;
    }

    shouldWork('周一') // 返回值是 上班
    shouldWork('周二') // 返回值是 上班
    shouldWork('周三') // 返回值是 上班
    shouldWork('周四') // 返回值是 上班
    shouldWork('周五') // 返回值是 上班
    shouldWork('周六') // 返回值是 上班
    shouldWork('周日') // 返回值是 上班
 
2、 function shouldWork(date) {
      var x;
var d=new Date().getDay();
switch (d)
  {
  case 0:
    x="上班";
    break;
  case 1:
    x="上班";
    break;
  case 2:
    x="上班";
    break;
  case 3:
    x="上班";
    break;
  case 4:
    x="上班";
    break;
  case 5:
    x="上班";
    break;
  case 6:
    x="上班";
    break;
  }
document.getElementById("demo").innerHTML=x;
    }

    shouldWork('周一') // 返回值是 上班
    shouldWork('周二') // 返回值是 上班
    shouldWork('周三') // 返回值是 上班
    shouldWork('周四') // 返回值是 上班
    shouldWork('周五') // 返回值是 上班
    shouldWork('周六') // 返回值是 上班
    shouldWork('周日') // 返回值是 上班
 ```
 ### 3) 补全下面的函数
 ``` 
  // 对 传入的所有参数求和
    function superAdd() {
      // 你写的内容
    }

    superAdd(1) // 返回值 1
    superAdd(1, 2) // 返回值 3
    superAdd(1, 2, 3, 4) // 返回值 10
    superAdd(1, 2, 3, 4, 5) // 返回值 15
 ```
 #### 答案
 ```
    function superAdd() {
   sum();
   var sum()=superAdd();
   ruturn 
      
    }

    superAdd(1) // 返回值 1
    superAdd(1, 2) // 返回值 3
    superAdd(1, 2, 3, 4) // 返回值 10
    superAdd(1, 2, 3, 4, 5) // 返回值 15
  ```
  ### 4) 补全下面的函数
  ```
    // 日期格式化
    function formateDate(date) {
      // 你写的内容
    }

    formateDate(new Date('2016/4/6')) // 返回值 2016年4月6日是星期四
  ```
  #### 答案
  ```
    function formateDate(date) {
      var date = new Date(date);
    return date.getFullYear()+"年"+(date.getMonth()+1)+"月"+date.getDate()+"日是"+date.Day;
    }

    formateDate(new Date('2016/4/6')) // 返回值 2016年4月6日是星期四
  ```
  ### 5) 编写函数反转字符串
  ```
   //编写reverse，满足如下条件
    reverse('abcd'); // 输出 'dbca'
    reverse('a'); // 输出 'a'
  ```
  #### 答案
  ```   
var h="abcd"   
var i=h.length;
i=i-1;  
for (var x = i; x >=0; x--)
{
document.write(h.charAt(x));  
}  
    reverse('abcd'); // 输出 'dbca'
    reverse('a'); // 输出 'a'
 ```
 ### 6) 统计字符串中各字符在字符串中出现的数量
 ```
 //编写caculateExistNum函数，满足如下条件
    caculateExistNum('abcd'); // 输出 {a:1,b:1,c:1,d:1}
    caculateExistNum('aaabbc00'); // 输出 {a:3,b:2,c:1,o:1}
    caculateExistNum(''); // 输出 {}
 ```
 ####  答案
 ```

    caculateExistNum('abcd'); // 输出 {a:1,b:1,c:1,d:1}
    caculateExistNum('aaabbc00'); // 输出 {a:3,b:2,c:1,o:1}
    caculateExistNum(''); // 输出 {}
 ```
 ### 7) 查找数组对象中 age 大于 18 对象
 ```
  // 编写filterAdult函数，满足如下条件
    filterAdult([
        {age: 19, name:'Jack'},
        {age: 5, name:'Apple'},
        {age: 12, name:'Lynn'},
        {age: 25, name:'David'}
    ]);
    // 输出
    [
        {age: 19, name:'Jack'},
        {age: 25, name:'David'}
    ]
 ```
 #### 答案
 
 
 
 ### 8) 将数组元素去重,其中数组元素均为基本类性
 ```
  //编写uniq函数，满足如下条件
    uniq([1,2,2,3,4,4,4,4]); // 输出 [1,2,3,4]
    uniq([1,2,'M','e','r', 'r', 'y']); // 输出 [1,2,'M','e','r','y']
 ```
 #### 答案
 ```
  function uniq(arr) {
      var newArr = [];
       var isUniq = true;
      for (i in arr) {
          for (j in newArr) {
              if (arr[i] === newArr[j]) {
                 isUniq = false;
              }
         }
          if (isUniq) {
            newArr.push(arr[i]);
         } else {
            isUniq = true;
         }
    }
     return newArr;
 }
  uniq([1,2,2,3,4,4,4,4]); // 输出 [1,2,3,4]
  uniq([1,2,'M','e','r', 'r', 'y']); // 输出 [1,2,'M','e','r','y']
```

    
