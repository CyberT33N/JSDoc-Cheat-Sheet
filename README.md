# JSDoc-Cheat-Sheet
JSDoc Cheat Sheet with the most needed stuff..

<br><br>

# DOCS
- https://jsdoc.app/index.html
















<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>


# Description
```javascript
/** This is a sample description.. */
async demo() {/*..*/};
```























<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>


# Paramater (@param)
```javascript
/**
 * Execute script inside of DOM by creating new function and run it
 * @param {string} script - Script - Script we want to execute
 * @param {object} page - Puppeteer page
 * @param {number|boolean} delay - Amount of time in ms we delay the execution
 * @param {function} anyFunction - A function that will be executed..
 * @param {boolean} access - If user has access or not
 *
 * @callback evalScriptCallback
 * @param {evalScriptCallback} cb - A callback to run.
*/
async evalScript(script, page, delay, anyFunction, access, cb) {
  anyFunction(delay, access);
  cb(script);
};
```


<br><br>


## Multiple paramater
```javascript
/**
 * Any fancy description
 * @param {number|boolean} delay - Amount of time in ms we delay the execution
*/
```


<br><br>


## Optional parameter
```javascript
/**
 @param {number} [foo]
 // or:
 @param {number=} foo
*/


/**
 * An optional parameter foo with default value 1.
 @param {number} [foo=1]
*/
```































<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>




# Return (@return)
```javascript
/**
 * @return {string} - Return demo which will be a string.
*/
async evalScript() {
/* do something.. */
return demo;
};
```

<br><br>


## return promises
```javascript
/**
 * @return {Promise<boolean>} - Will resolve with true.
*/
example() {return new Promise(resolve => {
/* do something.. */
resolve(true);
});};
```





















<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>




# @typedef (https://jsdoc.app/tags-typedef.html)
- The @typedef tag is useful for documenting custom types, particularly if you wish to refer to them repeatedly. These types can then be used within other tags expecting a type, such as @type or @param.
```javascript
/**
 * A number, or a string containing a number.
 * @typedef {(number|string)} NumberLike
 */

/**
 * Set the magic number.
 * @param {NumberLike} x - The magic number.
 */
function setMagicNumber(x) {
}
```

<br><br>

















































<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>




# destructuring
```javascript
/**
 * My cool function.
 *
 * @param {Object} obj - An object.
 * @param {string} obj.prop1 - Property 1.
 * @param {string} obj.prop2 - Property 2.
 */
var fn = function ({prop1, prop2}) {
  // Do something with prop1 and prop2
}
```

































<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>

# callback
```javascript
/**
 * Callback for adding two numbers.
 *
 * @callback addStuffCallback
 * @param {int} sum - An integer.
 */

/**
 * Add two numbers together, then pass the results to a callback function.
 *
 * @param {int} x - An integer.
 * @param {int} y - An integer.
 * @param {addStuffCallback} callback - A callback to run.
 */
function addStuff(x, y, callback) {
  callback(x+y);
}
```










