## 第3章
```html
<html>
    <head>
        <script src="https://code.jquery.com/jquery-3.6.0.js" 
          ntegrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk=" 
          crossorigin="anonymous">
        </script>
    </head>
    <body>
        <p>
            はじめてのプログラミング
        </p>
        <script>
            $('p').on('click', function(){
                $('p').text('変更後の文字列だよ〜ん！');
            });
        </script>
    </body>
</html>
```