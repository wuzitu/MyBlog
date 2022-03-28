---
title: 字节web面试题分享
date: 2022-03-28 21:41:39
tags: [web, 面试, 八股文]
categories: [面试,web]
description: 基础知识重点考察，项目经验也很重要。
---

# 问题1：问一个通信工程专业的问题。TCP的全称是什么，为什么能够保证完整性？UDP是什么，它有什么特点，和TCP各适用哪些场景？

# 问题2：jQuery和Vue最大的区别是什么，

# 问题3：讲一讲对HTTP2.0的认识

# 问题4：讲一讲HTTPS

# 问题5：实现one、two、add函数，
使得one(add(two())) 或two(add(one()))等于3

题目描述
```javascript
console.log(one(add(two())))//3
console.log(two(add(one())))//3
```
# 问题6：输出结果
```javascript
q = new Promise((resolve, reject) => {
    console.log(3);
    let p = new Promise((resolve, reject) => {
        console.log(7);
        setTimeout(() => {
            console.log(5);
            resolve(6);
        }, 0)
        resolve(1);
    });
    resolve(2);
    p.then((arg) => {
        console.log(arg);
    });
}).then((arg) => {
    console.log(arg);
});
console.log(4);
```

# 问题7：输出A结果，说明原因
```javascript
console.log(a)
function a() {
    console.log('a')
}
vara = 1
console.log(a)
function b() {
    console.log(a)
    leta = 2
}
b()
```

[更多2021高频面试题汇总](https://juejin.cn/post/6940945178899251230 "2021高频面试题汇总")