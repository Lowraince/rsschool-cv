# **Nazarov Vlad**

Junior Frontend Developer

### Contact information:

Email: *neson@yahoo.com*  
Discord: *lowraince*

---
### About me:
I want to try myself in programming and learn something new and interesting.

---
### Skills and Proficiency:
- HTML (basic)
- CSS (basic)
- JavaScript (basic)

---
### Code example:

```js
function highest(arr){
    const newArr = arr.reduce((acc, curr) => {
      acc[curr] = (acc[curr] || 0) + 1
    return acc
    }, {})
    
    const arrSort = Object.entries(newArr).sort(([, value],[,value2]) => value2 - value)
    
    const maxValue = arrSort[0][1]
    
    const arrF = arrSort.filter(([, value]) => value >= maxValue)

    const arrSort2 = arrF.sort(([key, value],[key2,value2]) => key2 - key)
    
    return +arrSort2[0][0]
}