# hhuanghuii.github.io
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        * {
            margin: 0;
            padding: 0;
        }
        
        body {
            min-width: 320px;
            max-width: 800px;
            margin: 0 auto;
            background-color: #ccc;
        }
        
        
        
        .app {
            width: 100%;
            height: 45px;
        
        }
        
        .app li {
            float: left;
            list-style: none;
            height: 45px;
            background-color: #333;
            text-align: center;
            color: #fff;
            line-height: 45px;
        }
        
        
        .app ul li:nth-child(1) {
            width: 8%;
            font-size: 30px;
        }
        
        
        .app ul li:nth-child(2) {
            width: 10%;
        
        }
        
        .app ul li:nth-child(2) img {
            width: 30px;
            border-radius: 5px;
            vertical-align: middle;
        }
        
        .app ul li:nth-child(3) {
            width: 57%;
        }
        
        .app ul li:nth-child(4) {
            width: 25%;
            background-color: #f63515;
        }
        
        .search {
            position: relative;
            width: 100%;
            height: 45px;
            overflow: hidden;
        }
        
        .search .search-menu {
            position: absolute;
            left: 0;
            top: 0;
            width: 45px;
            height: 44px;
            background-color: transparent;
            text-align: center;
        }
        
        #menu-icon {
            margin-top: 10px;
        }
        
        .search .search-menu img {
            display: block;
        
        }
        
        
        .search .search-login {
            position: absolute;
            right: 0;
            top: 0;
            width: 45px;
            height: 44px;
        
            color: #fff;
            text-align: center;
            line-height: 44px;
        }
        
        .search .search-box {
            position: relative;
            height: 30px;
            margin: 7px 60px 0 60px;
            background-color: #fff;
            border-radius: 15px;
        }
        
        .search .search-box .jd {
            position: absolute;
            width: 20px;
            height: 20px;
            background: url(../stu/jd.jpg) no-repeat;
            background-size: 20px 20px;
            left: 10px;
            top: 5px;
        
        }
        .jd::before {
            content: "";
            display: block;
            width: 1px;
            height: 18px;
            background-color: #ccc;
            margin-left: 25px;
        }
        #search-icon{
            position: absolute;
            top: 5px;
            left: 40px;
        }  
    </style>
</head>

<body>
    <!-- 头部 -->
    <header class="app">
        <ul>
            <!-- ×返回字体 -->
            <li>×</li>
            <!-- 京东图片 -->
            <li>
                < img src="D:\index\index.ts\stu\jingdong.jpg" alt="">
            </li>
            <li>打开京东APP，购物更轻松</li>
            <li>立即打开</li>
        </ul>
    </header>
    <!-- 整个搜索框盒子 -->

    <div class="search">
        <!-- 京东菜单图标 -->
        <div class="search-menu">
            <svg t="1613053433110" class="icon" id="menu-icon" viewBox="0 0 1024 1024" version="1.1"
                xmlns="http://www.w3.org/2000/svg" p-id="3222" width="28" height="28">
                <path
                    d="M124.56604 259.591293l0 84.975347 764.78119 0 0-84.975347L124.56604 259.591293zM124.56604 557.00603l764.78119 0 0-84.97637L124.56604 472.02966 124.56604 557.00603zM124.56604 769.44542l764.78119 0 0-84.97637L124.56604 684.46905 124.56604 769.44542z"
                    p-id="3223" fill="#000000"></path>
            </svg>
        </div>
        <!-- 京东搜索框 -->
        <div class="search-box">
            <!-- 搜索框里的JD图标 -->
            <div class="jd"></div>
            <!-- 搜索图标 -->
            <svg t="1613101286009" class="icon" id="search-icon" viewBox="0 0 1024 1024" version="1.1"
                xmlns="http://www.w3.org/2000/svg" p-id="2245" width="18" height="18">
                <path
                    d="M480 832A352 352 0 1 1 832 480 352.64 352.64 0 0 1 480 832z m0-640A288 288 0 1 0 768 480 288.64 288.64 0 0 0 480 192z"
                    fill="#4D4D4D" p-id="2246"></path>
                <path
                    d="M896 928a33.28 33.28 0 0 1-22.4-8.96l-192-184.96a32 32 0 0 1 44.16-46.08l192 184.96a32 32 0 0 1-21.76 55.04z"
                    fill="#4D4D4D" p-id="2247"></path>
            </svg>
            <!--  -->


        </div>
        <div class="search-login">
            登录
        </div>
    </div>

</body>

</html>
