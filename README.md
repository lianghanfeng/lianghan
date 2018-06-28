# lianghanfeng
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<meta name="viewport" content="width=device-width,initial-scale=1.0,maximum-scale=1.0,minimum-scale=1.0,user-scalable=no"> 
		<title>问题</title>
		<style>
			body{
				width: 100%;
				height: 100vh;
				overflow: auto;
			}
			div{
				width: 62%;
				margin-top: 40%;
				margin: auto;
			}
			div button{
				width: 80px;
				height: 50px;
				font-size: 20px;
			}
			h1{
				font-size: 1.5rem;
			}
			p{
				font-size: 0.8rem;
			}
		</style>
	</head>
	<body>
		<div>
			<h1>如果再给你一次选择的机会，那就还会不会理我？</h1>
			<p id="p"></p>
			<button id="yes">会</button>
			<button id="no">不会</button>
		</div>
	</body>
	<script>
		window.onload=function(){
			var yes=document.getElementById("yes");
			var no=document.getElementById("no");
			var p=document.getElementById("p");
			yes.onclick=function(){
				alert("我一定会理你的，我承诺过的事肯定会做到");
			}
			
			var z=new Array("怎么？还要不理我啊？","别不理我啊，之前是有点生气","我可是跟你承诺过的","哼，那我消失了","还不理我，真消失了","消失，看你理不理我，哼");
			var i=0
			no.onclick=function(){
				p.innerHTML +=z[i]+"<br>";
				if(i>4){
					this.style.display="none";
				}else{
					i++;
				}
			}
		}
	</script>
</html>
