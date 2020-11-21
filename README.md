# hhuanghuii.github.io
<html>
<head> 
<meta charset="utf-8"> 
<title></title> 
<style>
.outbox{
 margin:auto;
 height:60px;
 width:160px;
 border: 3px solid black;
 border-radius: 30px;
 }
.insidebox{
 width:46px;
 height:46px;
 border:3px solid black;
 border-radius:100%;
 margin-left:7px;
 margin-top:3px;
 box-shadow: 6px -5px 0 3px #ff81ff inset;
  
 }
 .focus{
  position:absolute;
  padding:300px;
 }
 .dot{
  width:8px;
  height:8px;
  background-color:blue;
  border-radius:100%;
 }
 .focus div[class^="ripple"]{
  position:absolute;
  top:50%;
  left:50%;
  transform: translate(-50%,-50%);
  border-radius:50%;
   width:1px;
  height:1px;
  
  box-shadow: 0 0 6px blue;
  animation:jiaodian 3s linear infinite;
  
 
 }
 @keyframes jiaodian{
  0%{}
  100%{width:60px; height:60px}
  
 }
 .ripple2{
  animation-delay:1s!important;
 }
 .ripple3{
  animation-delay:2s!important;
 }
</style>
</head>
<body>
 
<form>
<select>
<option value="黄">黄</option>
<option value="梁">梁</option>
<option value="陈">陈</option>
<option value="胡">胡</option>
</select>
</form>
<input type="range">
<input type=-"color">

<div class="outbox">
 <div class="insidebox"></div>
</div>
<div class="focus">
 <div class="dot">
  <div class="ripple1"></div>
  <div class="ripple2"></div>
  <div class="ripple3"></div>
 </div>
 

</div>
 
 
 
</body>
</html>

