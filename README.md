
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
h1 {
  color: #ffffff;
  font-size: 40px;
  text-align: center;
}
h2 {
  font-size: 20px;
  color: #ffffff;
  text-align: center;
}
.countdown {
  position: relative;
  margin: 300px auto;
  width: 200px;
  height: 300px;
  background-color: #2ca9ad;
  border-radius: 10px;
}
.day {
  position: absolute;
  margin: 0 auto;
  width: 40px;
  height: 30px;
  background-color: gray;
  color: white;
  line-height: 30px;
}
.hours {
  position: absolute;
  font-size: 20px;
  text-align: center;
  left: 52px;
  bottom: 15px;
  display: inline-block;
  width: 30px;
  height: 35px;
  background-color: gray;
  color: white;
  line-height: 35px;
}
.min {
  position: absolute;
  font-size: 20px;
  text-align: center;
  bottom: 15px;
  right: 85px;
  display: inline-block;
  width: 30px;
  height: 35px;
  background-color: gray;
  color: white;
  line-height: 35px;
}
.sec {
  position: absolute;
  font-size: 20px;
  text-align: center;
  bottom: 15px;
  right: 52px;
  display: inline-block;
  width: 30px;
  height: 35px;
  background-color: gray;
  color: white;
  line-height: 35px;
}
.icon {
  position: absolute;
  top: 155px;
  right: 76px;
}
p {
  position: absolute;
  top: 210px;
  left: 20px;
  color: #ffffff;
}
    </style>
</head>
<body>
    <div class="countdown"> 
        <h1>Birthday</h1>
        <h2>countdown</h2>
        <svg t="1619570366163" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="1349" width="48" height="48"><path d="M784.222 793.944V385.611H667.556V249.5h-58.333v136.111h-68.056V249.5h-58.333v136.111h-68.056V249.5h-58.333v136.111H239.778V793.944H162v58.333h700v-58.333h-77.778z m-58.333 0H298.111v-167.82l7.925 7.925 41.248-41.248 41.248 41.248 41.247-41.248 41.248 41.248 41.247-41.248 41.248 41.248 41.248-41.248 40.698 40.698 41.248-41.248 41.248 41.248 7.923-7.925v168.37z m0-250.864l-7.923 7.923-41.248-41.248-41.248 41.248-40.698-40.698-0.551-0.551-41.248 41.248-40.698-40.698-41.247 41.248-41.248-41.248-41.247 41.248-41.248-41.248-41.248 41.248-7.925-7.925v-99.684H725.89v99.137zM356.444 171.722h58.333v58.333h-58.333zM482.833 171.722h58.333v58.333h-58.333zM609.222 171.722h58.333v58.333h-58.333z" p-id="1350" fill="#ffffff"></path></svg>
        <p></p>
        <div class="hours"></div>
        <div class="min"></div>
        <div class="sec"></div>
    </div>
</body>
<script>
    var daybox = document.querySelector('.day');
	var hoursbox = document.querySelector('.hours');
	var minbox = document.querySelector('.min');
	var secbox = document.querySelector('.sec');
	var textcount = document.querySelector('p');
	var birthday = prompt('输入你的生日');
function count() {
    var nowtime = +new Date();
    var birtime = +new Date(birthday);
    var overtime = (birtime - nowtime)/1000;

    var sec = parseInt(overtime % 60);
    sec = sec < 10 ? '0' + sec : sec;
    secbox.innerHTML = sec;

    var min = parseInt(overtime / 60 % 60);
    min = min < 10 ? '0' +min : min;
    minbox.innerHTML = min;
    
    var hours = parseInt(overtime / 60 / 60 %24);
    hours = hours < 10 ? '0' + hours :hours;
    hoursbox .innerHTML = hours;

    var day = parseInt(overtime /60 / 60 / 24);
    day = day < 10 ? '0' + day : day;

    textcount.innerHTML = '距离你的生日还剩' + day + '天';
}
count();
setInterval(() => {
    count();
}, 1000);
</script>
</html>       
