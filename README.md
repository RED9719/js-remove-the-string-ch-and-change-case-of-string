# js-remove-the-string-ch-and-change-case-of-string

. Write a JavaScript program to 
a) Remove a character at the specified position of a given string and return the new string. 
CODE
          <!DOCTYPE html>
<html>
<head>
    <title>Remove Character at Specified Position</title>
    <script>
        function removeCharacterAtPosition(str, position) {
            if (position < 0 || position >= str.length) {
                return str; 
            }
            return str.slice(0, position) + str.slice(position + 1);
        }
        window.onload = function() {
            const originalString = "Ramanujan";
            const position = 3;
            const newString = removeCharacterAtPosition(originalString, position);
            console.log("Original string:", originalString); 
            console.log("New string:", newString); 
        }
    </script>
</head>
<body>
    <h1>Check the console for the result</h1>
</body>
</html>
 
b) Change the case of a string. (I.e. upper case to lower case and vice-versa). 
CODE
         <!DOCTYPE html>
<html>
<head>
    <title>Change Case of String</title>
    <script>
        function changeCase(str) {
            let newStr = '';
            for (let i = 0; i < str.length; i++) {
                if (str[i] === str[i].toUpperCase()) {
                    newStr += str[i].toLowerCase();
                } else {
                    newStr += str[i].toUpperCase();
                }
            }
            return newStr;
        }
        window.onload = function() {
            const originalString = "RaMaNuJaN CoLlEgE";
            const changedString = changeCase(originalString);
            console.log("Original string:", originalString);
            console.log("Changed string:", changedString);  
        }
    </script>
</head>
<body>
    <h1>Check the console for the result</h1>
</body>
</html>
