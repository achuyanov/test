# [test](https://www.tut.by)
```js
let getCellRangeFunc = this.getCellRange;
return function(workSheet, range){
    const dataFromExcel = getCellRangeFunc(workSheet, range)
    const dataFromExcelLength = dataFromExcel.length
    let obj = {}
    for (let i = 0; i < dataFromExcelLength; i++) {
        let subArray = dataFromExcel[i]
        if (subArray.length > 1) obj[subArray[0]] = subArray[subArray.length-1]
    }
    return obj;
}
```
# Andrei Chuyanov
---
##Contact:

email: achuyanov@gmail.com
skype: andrei.chuyanov
mobile: +375297540133
