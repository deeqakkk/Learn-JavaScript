<h1 align="center">Strings Methods</h1>

### 1. charCodeAt()
The charCodeAt() method returns the Unicode(an integer between 0 and 65535) of the character at the specified index in a string.
```js
const str = 'Deepak';

console.log(str.charCodeAt(0)); // returns 68
```
### 2. concat()
The concat() method is used to join two or more strings.
```js
const str1 = 'Deepak';
const str2 = 'Verma';

console.log(str1.concat(str2)); // returns DeepakVerma
```
### 3. length property
The length property returns the length of a string.
```js
const str = 'Deepak';

console.log(str.length); // returns 6
```
### 4. slice(start, end)
The slice() method extracts a part of a string and returns the extracted part in a new string.
```js
const str = 'Deepak Verma is a fullstack MERN Developer';

console.log(str.slice(20)); // "llstack MERN Developer"
console.log(str.slice(4,20)); // "ak Verma is a fu"
console.log(str.slice(-7)); // "veloper"
console.log(str.slice(-9, -5)); // "Deve"
```
### 5. substring(start, end)
The substring() method extracts the characters from a string, between two specified indices, and returns the new sub string.
```js
const str = 'Deepak';
console.log(str.substring(0,3)); // "Dee"
console.log(str.substring(3)); // "pak"
```
### 6. at()
The at() method returns the character at the specified index in a string.
```js
const sentence = 'Deepak Verma';

// positive index will return character from start
console.log(sentence.at(3)); // p
// negative index will return character from end
console.log(sentence.at(-3)); // r
```

### 7. endsWith()
The endsWith() method determines whether a string ends with the characters of a specified string, returning true or false as appropriate.
```js
const str = 'Deepak Verma is a good boy!';

console.log(str.endsWith('boy!')); // true
console.log(str.endsWith('boy')); // false
```

### 8. includes()
The includes() method determines whether one string may be found within another string, returning true or false as appropriate.
```js
const str='Valorant is a 5 multiplayer FPS game';

console.log(str.includes('FPS')); // true
console.log(str.includes('fps')); // false
```

### 9. indexOf()
The indexOf() method returns the index of the first occurrence of the specified value, starting the search at fromIndex. Returns -1 if the value is not found.
```js
const str = 'Deepak loves to play valorant along with his two friends!';
console.log(str.indexOf('along')); //30
console.log(str.indexOf('loves')); //7
console.log(str.indexOf('deepak')); //-1
console.log(str.indexOf('Deepak')); //0
```

### 10. lastIndexOf()
The lastIndexOf() method returns the last occurrence of the specified value, or -1 if not found.
```js
const str = 'Deepak verma Deepak writes on js on twitter. deepak also loves to read books';

console.log(str.lastIndexOf('deepak'));  //45
console.log(str.lastIndexOf('Deepak'));  //13
console.log(str.lastIndexOf('DeepakVerma')); //-1
```
### 11. padEnd()
The padEnd() method pads the current string with a given string (repeated, if needed) so that the resulting string reaches a given length. The padding is applied from the end of the current string.
```js
const str = 'Deepak';
console.log(str.padEnd(10, '1')); //"Deepak1111"

const str2 = 'Verma';
console.log(str2.padEnd(10));  //"Verma     "
```

### 12. padStart()
The padStart() method pads the current string with another string (multiple times, if needed) until the resulting string reaches the given length. The padding is applied from the start of the current string.
```js
console.log("Deepak".padStart(10)); // "    Deepak"
console.log("Verma".padStart(10, "Dee")); // "DeeDeVerma"
console.log("Verma".padStart(6, "@")); // "@Verma"
console.log("deepak".padStart(8, "#")); // "##deepak"
console.log("Deepak".padStart(1)); // "Deepak"
```
### 13. repeat()
The repeat() method constructs and returns a new string which contains the specified number of copies of the string on which it was called, concatenated together.
```js
const name = '@deeqakkk';

console.log(name.repeat(4)); //"@deeqakkk@deeqakkk@deeqakkk@deeqakkk"
console.log(name.repeat(0)); //""
console.log(name.repeat(1)); //"@deeqakkk"
console.log(name.repeat(2.5)); //"@deeqakkk@deeqakkk"
```
### 14. toLowerCase()
The toLowerCase() method returns the calling string value converted to lower case.
```js
const str = 'DEEPAK';
console.log(str.toLowerCase()); // "deepak"
```
### 15. toUpperCase()
The toUpperCase() method returns the calling string value converted to uppercase (the value will be converted to a string if it isn't one).
```js
const str = 'deepak';
console.log(str.toUpperCase()); // "DEEPAK"
```
### 16. trim()
The trim() method removes whitespace from both ends of a string.
```js
const name = '  Deepak  ';
console.log(name.trim()); // "Deepak"
```

### 17. trimEnd()
The trimEnd() method removes whitespace from the end of a string.
```js
const name = 'Deepak  ';
console.log(name.trimEnd()); // "Deepak"
```
### 18. trimStart()
The trimStart() method removes whitespace from the beginning of a string.
```js
const name = '  Deepak';
console.log(name.trimStart()); // "Deepak"
```