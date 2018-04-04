# helper-js
js functions, just import needed functions.   
js 方法库, 按需使用   

```sh
// install
npm install helper-js -S
```
### usage 使用
```
import {function1, function2} from'helper-js

```
### some functions. pls check source to get more 常用方法, 请查看源码获取更多方法
###### isset   
typeof v !== 'undefined'
###### isArray   
Object.prototype.toString.call(v) === '[object Array]'
###### isBool   
###### isNumber   
###### isNumeric   
###### isString   
###### isObject   
###### isFunction   
###### isPromise   
###### numRand   (min, max) // get a rand integer, include min and max
###### numPad(num, n)
(10, 3) => '010', (2, 4) => '0002'
###### min(n, min)
(1, 10) => 10, (11, 10) => 11
###### max(n, max)
(1, 10) => 1, (11, 10) => 10
###### studlyCase
hello => Hello
###### kebabCase   
helloWorld nice => hello-world-nice
###### snakeCase
helloWorld nice => hello_world_nice
###### camelCase   
helloWorld nice => helloWorldNice
###### camelToWords   
helloWorldNice => hello World nice
###### titleCase   
helloWorldNice => Hello World Nice
###### strRand   (len = 8, prefix = '')
###### replaceMultiple (mapObj, str)
({'1': '2', '3': '4'}, 'abcd1234') => 'abcd2244'
###### arrayRemove   (arr, item) // remove any === item
###### arrayFirst   
###### arrayLast   
###### arrayDiff  (arr1, arr2) // return items in arr2 but not in arr1
###### toArrayIfNot   
###### assignIfDifferent(obj, key, val)   
###### objectMerge (obj1, obj2) // merge obj2 to obj1, and merge obj2 chldren to obj1 if it is object
###### objectMap   (obj, func)
###### objectOnly   (obj, keys) // return new object
###### objectExcept   (obj, keys) // return new object
###### objectGet   (obj, path, defaultValue = null) // get by dot path
({a:{b:1}}, 'a.b') => 1
###### objectSet   (obj, path, value)
###### unset (obj, prop)
###### cloneObj  (obj, exclude) // exclude: array or function
###### executeWithCount (func, context = null) // wrap function, last arg of new function is excuted count
###### watchChange   (getVal, handler) // wrap getter function, when use getter to get value, it will check value if changed
###### getUrlParam   // get current url param by name
##3 DOM
###### uniqueId  (prefix = 'id_') // html element id
###### isDescendantOf (el, parent)  // if el === parent or is descendant of parent
###### getOffsetWithoutScroll   // get offset({x,y}) of an el
###### getOffset   
###### findParent (el, callback)
###### backupAttr   (el, name)
###### restoreAttr   (el, name)
###### hasClass   (el, className)
###### addClass   (el, className)
###### removeClass   (el, className)
###### getElSize   (el)
###### isOffsetInEl   (x, y, el)
###### getBorder   (el) // return {left, top, right, bottom}
###### setElChildByIndex   
###### onDOM (el, name, handler)   // addEventListener
###### offDOM (el, name, handler)   // removeEventListener
###### binarySearch   (arr, callback, start, end, returnNearestIfNoHit, max = 1000) // binary search 二分查找
###### windowLoaded   // return a promise
###### waitFor   (name, condition, time = 100, maxCount = 1000)
###### retry   (func, limitTimes = 3)
###### copyTextToClipboard   (text) // tested in chrome
### jquery
###### jqFixedSize   
###### jqMakeCarousel