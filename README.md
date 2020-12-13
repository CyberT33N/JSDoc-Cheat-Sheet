# JSDoc-Cheat-Sheet
JSDoc Cheat Sheet with the most needed stuff..

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
 * @param {number} delay - Amount of time in ms we delay the execution
*/
async evalScript(script, page, delay) {/*..*/};
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
