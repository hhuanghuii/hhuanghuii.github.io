<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .count{
            position: relative;
            margin: 200px auto;
            width: 200px;
            height: 250px;
            border-radius: 20px;
            background:linear-gradient(30deg, rgb(27, 201, 224), rgb(62, 187, 110));
            box-sizing: border-box;
        }
        .textcount{
            height: 40px;

            border-radius: 5px;
            font-size: 20px;
            margin: 0 auto;
            text-align: center ;
            line-height: 40px;
            color: white;
        }
        h1{
            color: white;
            font-size: 30px;
            text-align: center;


        }
        .hours{
            position: absolute;
            font-size: 20px;
            color: white;
            bottom: 15px;
            left: 53px;
            width: 30px;
            height: 30px;
            background-color: rgb(133, 132, 131);
            border-radius: 5px;
            text-align: center;
            line-height: 30px;
        }
        .min{
            position: absolute;
            font-size: 20px;
            color: white;
            bottom: 15px;
            right: 85px;
            width: 30px;
            height: 30px;
            background-color: rgb(133, 132, 131);
            border-radius: 5px;
            text-align: center;
            line-height: 30px;
        }
        .sec{
            position: absolute;
            font-size: 20px;
            color: white;
            bottom: 15px;
            right: 53px;
            width: 30px;
            height: 30px;
            background-color: rgb(133, 132, 131);;
            border-radius: 5px;
            text-align: center;
            line-height: 30px;
        }
        p{
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="count">
        <h1>Birthday</h1>
        <p><svg t="1619623138248" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="4386" width="50" height="50"><path d="M784.222 793.944V385.611H667.556V249.5h-58.333v136.111h-68.056V249.5h-58.333v136.111h-68.056V249.5h-58.333v136.111H239.778V793.944H162v58.333h700v-58.333h-77.778z m-58.333 0H298.111v-167.82l7.925 7.925 41.248-41.248 41.248 41.248 41.247-41.248 41.248 41.248 41.247-41.248 41.248 41.248 41.248-41.248 40.698 40.698 41.248-41.248 41.248 41.248 7.923-7.925v168.37z m0-250.864l-7.923 7.923-41.248-41.248-41.248 41.248-40.698-40.698-0.551-0.551-41.248 41.248-40.698-40.698-41.247 41.248-41.248-41.248-41.247 41.248-41.248-41.248-41.248 41.248-7.925-7.925v-99.684H725.89v99.137zM356.444 171.722h58.333v58.333h-58.333zM482.833 171.722h58.333v58.333h-58.333zM609.222 171.722h58.333v58.333h-58.333z" p-id="4387" fill="#ffffff"></path></svg></p>
        <div class="textcount"></div>
        <div class="hours"></div>
        <div class="min"></div>
        <div class="sec"></div>
    </div>
</body>
<script>
    var h = document.querySelector('.hours');
    var m = document.querySelector('.min');
    var s = document.querySelector('.sec');
    var textcount = document.querySelector('.textcount');
    


    function count() {
        var nowtimes = +new Date();
        var bir = +new Date('2021-5-2');
        var overtime = (bir - nowtimes) / 1000; 

        var sec = parseInt(overtime % 60);
        sec = sec < 10 ? '0' + sec : sec;


        var min = parseInt(overtime / 60 % 60);
        min = min < 10 ? '0' + min : min;


        var hours = parseInt(overtime / 60 /60 % 24);
        hours = hours < 10 ? '0' + hours : hours;


        var day = parseInt(overtime /60 / 60 /24);
        day = day < 10 ? '0' + day : day;

        textcount.innerHTML = day + '天' + hours + ':' + min + ':' + sec
    } 
    count()
    setInterval(() => {
        count();
    }, 1000);
    
</script>
</html>
