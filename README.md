<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" type="text/css" href="ym.css">  
</head>
<body>
    <div id="div-title">
        <h3>欢迎登录</h3>
    </div>
    <div id="form-border">
        <form action='shouy.html'onsubmit="return f()">
            <div id="img-control">
                <img src="img/zhuce.jpg" id="login-img">
            </div>
            <label class="from-label" for="account">账&nbsp;号</label>
            <input id="account" class="form-input" type="text" placeholder="请输入账号" required="required"><br>
            <label class="from-label" for="password">密&nbsp;码</label>
            <input id="password" class="form-input" type="password" placeholder="请输入密码" required="required"><br>
            <label id="register" class="form-label" for="password">没有账号？<a href="register.html">点击注册</a></label><br>
            <input id="login" class="form-button" type="submit" value="登录">
            <input id="reset" class="form-reset" type="reset" value="重置"><br>
        </form>
        <script>
            function f() {
                var flat = true;
                var myUerName = document.querySelectorAll("input")[0];
                var myPassWord = document.querySelectorAll("input")[1];
                if (myUerName.value == "123456") {
                    if (myPassWord.value == "666666") {
                        alert("验证成功！");
                        return flat;
 
                    } else {
                        flat = false;
                        alert("密码错误，请重新输入！");
                        return flat;
                    }
                } else {
                    flat = false;
                    alert("用户名错误，请重新输入！");
                    return flat;
                }
            }
        </script>
    </div>
</body>
</html>
