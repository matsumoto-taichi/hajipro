## 第6章
### 6.1.1
```html
<html>
    <script>
        window.alert('はじめてのJavaScript！');
    </script>
</html>
```

### 6.1.2
```html
<html>
    <header>
        <script src="https://code.jquery.com/jquery-3.6.0.js" 
          ntegrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk=" 
          crossorigin="anonymous">
        </script>
    </header>
    <body>
        <p style="font-size: xx-large;">
            Hello World！
        </p>
    </body>
    <script>
        $('p').on('click', function(){
            window.alert($('p').text());
        });
    </script>
</html>
```

### 6.1.3
```html
<html>
    <head>
        <script src="https://code.jquery.com/jquery-3.6.0.js" 
          ntegrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk=" 
          crossorigin="anonymous">
        </script>
    </head>
    <body>
        <p style="font-size: xx-large;">
            Hello World！
        </p>
    </body>
    <script>
        $('p').on('click', function(){
            window.alert($('p').text());
            window.alert($('p').text());
            window.alert($('p').text());
        });
    </script>
</html>
```

### 6.2.1
```html
<html>
    <body>
        <button>
            押してください！
        </button>
    </body>
</html>
```

### 6.2.2
```javascript
function message(){
    window.alert("ボタンが押されました！");
}  
```

### 6.2.3
```html
<html>
    <body>
        <button onclick="message()">
            押してください！
        </button>
    <script>
        function message(){
            window.alert("ボタンが押されました！");
        }
    </script>
    </body>
</html>
```

### 6.3.1
```html
<html>
    <body>
        <div style="background-color: cyan; width: 300px; height: 100px; border: black solid 2px ">
        </div>
    </body>
</html>
```

### 6.3.2
```html
<html>
    <head>
    <script src="https://code.jquery.com/jquery-3.6.0.js"
            ntegrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk="
            crossorigin="anonymous">
    </script>
    </head>
    <body>
        <div id="shikaku" style="background-color: cyan; width: 300px; height: 100px; border: black solid 2px ">
        </div>
        <script>
            $('#shikaku').on('click',function() {
                $('#shikaku').animate({
                    'marginTop': '400px',
                    'marginLeft': '900px'
                },
                1000);
            });
        </script>
    </body>
</html>
```
```html
<html>
    <head>
        <script src="https://code.jquery.com/jquery-3.6.0.js" 
          ntegrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk=" 
          crossorigin="anonymous">
        </script>
    </head>
    <body>
        <body>
            <button onclick="start()">
                押してください！
            </button>
        </body>
        <div id="shikaku" style="background-color: cyan; width: 300px; height: 100px; border: black solid 2px;">
        </div>
        <script>
            start = function() {
                $('#shikaku').animate({
                        'marginTop': '400px',
                        'marginLeft': '900px'
                    },
                    1000);
            }
        </script>
    </body>
</html>
```

### 6.3.3
```html
<html>
    <head>
        <script src="https://code.jquery.com/jquery-3.6.0.js" 
          ntegrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk=" 
          crossorigin="anonymous">
        </script>
    </head>
    <body>
        <body>
            <button onclick="start()">
                押してください！
            </button>
        </body>
        <div id="shikaku" style="background-color: cyan; width: 300px; height: 100px; border: black solid 2px;">
        </div>
        <script>
            start = function() {
                $('#shikaku').animate({
                        'marginTop': '400px',
                        'marginLeft': '900px'
                    },
                    1000);
                $('#shikaku').css({'background-color': 'pink'});
            }
        </script>
    </body>
</html>
```

