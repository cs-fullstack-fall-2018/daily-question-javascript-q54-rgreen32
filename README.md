# Daily question MS-54

### Let, Const
MSJS practice question 54

```
You preview the following page in the browser:

<!DOCTYPE html>
<html>
<head>
    <title>Intro to JavaScript</title>
	<meta charset="utf-8" />
    <style>
        .format-output {
            width: 300px;
            height: 100px;
            border: 1px solid blue;
            font:bold 20px "courier new";
            text-align:center;
        }
    </style>
</head>
<body>
    <div id="result" class="format-output"></div>
    <script>
        let names = ['Apple', 'Orange', 'Banana', 'Kiwi'];

        {
            let names = ['Blue', 'Green', 'Orange', 'Yellow', 'Red'];

            function findIndex(element) {
                if (!element) return;
                for (var i = 0; i < names.length; i++) {
                    if (names[i].toLowerCase() === element.toLowerCase())
                        return i;
                }
            }
        }

        function getBefore(i) {
            if (i <= 0) return;
            return names[i - 1];
        }
        
        names.sort();
        var index = findIndex('orange');

        document.getElementById("result").innerHTML = getBefore(index);
    </script>
</body>
</html>
```

* Which word will be displayed on the screen?

1) Yellow

2) Green	X

3) Banana

4) Kiwi



