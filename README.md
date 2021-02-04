# JSDoc-Cheat-Sheet
JSDoc Cheat Sheet with the most needed stuff..

<br><br>

# DOCS
- https://jsdoc.app/index.html


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
 * @param {number} delay - Amount of time in ms we delay the execution
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


## destructuring
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
