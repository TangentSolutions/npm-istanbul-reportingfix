## Istanbul - a JS code coverage tool written in JS - reporting fix

### Overview

This is a fix to the original [Istanbul](https://github.com/gotwarlost/istanbul) while this issue is resolved on their side. :)

### What we fixed
Changed condition for istanbul in file /lib/report/html.js,
fix for error: ERROR [coverage]: TypeError: Cannot read property 'text' of undefined
Changes Made:
line 205: if (type === 'no') changed to if (type === 'no' && structuredText[startLine])
line 236: if (type === 'no') changed to if (type === 'no' && structuredText[startLine])

### Installation

Include the following in your `package.json` file

     "istanbul": "git+https://github.com/TangentSolutions/npm-istanbul-reportingfix.git",
