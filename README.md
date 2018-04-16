<!DOCTYPE HTML>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Title</title>
        <meta name="keywords" content="关键词">
        <meta name="description" content="描述">
        <meta name="author" content="九年与十年">
        <style>
            body,dl,dd,p,h1,h2,h3,h4,h5,h6{margin:0;}
            ol,ul,li{margin:0;padding:0;list-style:none;}
            img{border:none;}
            #wrap{
                position: absolute;
                top: 0;
                width: 50px;
                height: 100%;
                background-color: #666;
            }
            #button{
                position: fixed;
                left: 0;
                bottom: 50px;
                width: 50px;
                height: 50px;
                background-color: #ececec;
            }
        </style>
    </head>
    <body>
        <div id="wrap">
            <div id="button"></div>
        </div>
        
        <script>
            var xwrap = document.getElementById("wrap"),
                button = document.getElementById("button"),
                x = true;
	            button.onclick = function() {
		            if (x) {
			            xwrap.style.left = "-50px";
		            } else {
			            xwrap.style.left = "0px";
			            alert(x)
		            }
		            x =! x;
	            }
        </script>
    </body>
</html>
