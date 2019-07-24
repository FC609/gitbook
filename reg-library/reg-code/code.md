# 有趣的正则片段

## `\1`
```javascript
let str = 'aaaaaaaabdddddhhhhhhhhijjjjjkkpsssssssu',
    reg = /(.)\1+/g,
    obj = {};
    str.replace(reg, (...arg) => {
            console.log(arg);
            obj[arg[1]] = arg[0].length
        });
console.log(JSON.stringify(obj)); // {"a":8,"d":5,"h":8,"j":5,"k":2,"s":7}
```
> 正则表达式中的小括号"()"。是代表分组的意思。 如果再其后面出现\1则是代表与第一个小括号中要匹配的内容相同。
> 
> <b>`注意：`</b>\1必须与小括号配合使用