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
 * @param {string} - Script - Script we want to execute
 * @param {object} - Puppeteer page
 * @param {number} - Amount of time in ms we delay the execution
*/
async evalScript(script, page, delay) {/*..*/};
```

# Return (@return)
```javascript
/**
 * @return {string} - Return demo which will be a string
*/
async evalScript() {
/* do something.. */
return demo;
};
```


<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>
