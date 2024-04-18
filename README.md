<html>
<head>
<title>This is why you came here</title>
<meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css" integrity="sha384-9aIt2nRpC12Uk9gS9baDl411NQApFmC26EwAOH8WgZl5MYYxFfc+NcPb1dKGj7Sk" crossorigin="anonymous">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<style>
.heartb{
	    position: relative;
	    width: 60px;
	    z-index:99999;
	    height: 50px;
	    left:25%;
	    animation: heart 1s infinite;
	    transform:scale(.8);
	    transition:.6s;
	    
	}
	.heartb:before,
	.heartb:after{
	    content: "";
	    width: 25px;
	    height: 40px;
	    position: absolute;
	    left: 25px;
	    top: 0;
	    border-radius: 50px 50px 6px 6px;
	    background: crimson;
	    transform: rotate(-45deg);
	    transform-origin: 0 100%;
	}
	.heartb:after{
	    left: 0;
	    transform: rotate(45deg);
	    transform-origin :100% 100%;
	}

	@keyframes heart {
	    0% {
	        transform: scale(.😎 translate(0,0);
	    }
	    
	    50% {
	        transform: scale(.92) translate(0, 12px);
	    }
	    
	    100% {
	        transform:scale(.8);
	    }
	}
	  
	.button-heart {
	  background: transparent; 
	  margin: auto;
	  height: 150px;
	  position: relative;
	  width: 150px;
	  border: none;
	  overflow:hidden;
	  animation: floaty 1s infinite;
	}

	@keyframes floaty {
	    0% {
	        transform:translate(0,0);
	    }
	    
	    50% {
	        transform:translate(0, 12px);
	    }
	}
/*added here*/
.bg_heart {
    position: relative;
    top: 0;
    left: 0;
    width: 100%;
    height: auto;
    overflow: hidden;
     }
.heart {
    position: absolute;
    top: -50%;
    -webkit-transform: rotate(-45deg);
    -moz-transform: rotate(-45deg);
    -m-transform: rotate(-45deg);
    transform: rotate(-45deg)
 }

.heart:before {
    position: absolute;
    top: -50%;
    left: 0;
    display: block;
    content: "";
    width: 100%;
    height: 100%;
    background: inherit;
    border-radius: 100%;
}

.heart:after {
    position: absolute;
    top: 0;
    right: -50%;
    display: block;
    content: "";
    width: 100%;
    height: 100%;
    background: inherit;
    border-radius: 100%;
}

@-webkit-keyframes love {
  0%{top:110%}
}
@-moz-keyframes love {
  0%{top:110%}
}
@-ms-keyframes love {
  0%{top:110%}
}
@keyframes love {
  0%{top:110%}
}
  </style>
</head>
<body >
<div class="bg_heart container-fluid">
<div class="container-fluid text-center head-plugin" style="background-color:#d86a77; ">
<div class="alert alert-danger">
  <strong>Danger!</strong> You will fall in love with me.
</div>  

<div class="embed-responsive embed-responsive-16by9">
<iframe class="embed-responsive-item" src="https://www.youtube.com/embed/aBFE7yn3lso" allow="encrypted-media;" allowfullscreen></iframe>
</div>
<div id="p-4">
<div  id="myBar"  class="progress-bar progress-bar-striped progress-bar-animated m-3 text-center bg-success">This is My love for You</div> 
<button onclick="move()" class="btn btn-success">Click Here to Find Your Love for ME</button> 
</div>
<div class="p-4">
<button type="button" class="btn  btn-danger p-4"><a href="https://m.me/100011457304911?ref=I_Love_You_Too" class="text-success">Accept my proposal</a></button>
</div>
	</div>
	</div>
	<div class="container text-center">
	<img src="heart.svg" id="lol">
	<br>
	<button onclick="startGame()" class="button-heart">
		<div class="heartb"> </div>
	</button>
</div>
<script>
	var x = 100 ;
	document.getElementById("lol").style.width = 100 +"%";
	document.getElementById("lol").style.height  = 100 + "%";
	document.getElementById("lol").style.opacity = 0.0 ;
     $( "#header-plugin" ).load( "https://vivinantony.github.io/header-plugin/", function() {
	$("a.back-to-link").attr("href", "http://blog.thelittletechie.com/2015/03/love-heart-animation-using-css3.html#tlt")  
});

var love = setInterval(function() {
    var r_num = Math.floor(Math.random() * 40) + 1;
    var r_size = Math.floor(Math.random() * 65) + 10;
    var r_left = Math.floor(Math.random() * 100) + 1;
    var r_bg = Math.floor(Math.random() * 25) + 100;
    var r_time = Math.floor(Math.random() * 5) + 5;

    $('.bg_heart').append("<div class='heart' style='width:" + r_size + "px;height:" + r_size + "px;left:" + r_left + "%;background:rgba(255," + (r_bg - 25) + "," + r_bg + ",1);-webkit-animation:love " + r_time + "s ease;-moz-animation:love " + r_time + "s ease;-ms-animation:love " + r_time + "s ease;animation:love " + r_time + "s ease'></div>");

    $('.bg_heart').append("<div class='heart' style='width:" + (r_size - 10) + "px;height:" + (r_size - 10) + "px;left:" + (r_left + r_num) + "%;background:rgba(255," + (r_bg - 25) + "," + (r_bg + 25) + ",1);-webkit-animation:love " + (r_time + 5) + "s ease;-moz-animation:love " + (r_time + 5) + "s ease;-ms-animation:love " + (r_time + 5) + "s ease;animation:love " + (r_time + 5) + "s ease'></div>");

    $('.heart').each(function() {
        var top = $(this).css("top").replace(/[^-\d\.]/g, '');
        var width = $(this).css("width").replace(/[^-\d\.]/g, '');
        if (top <= -100 || width >= 150) {
            $(this).detach();
        }
    });
}, 500);
var i = 0;
function move() {
  if (i == 0) {
    i = 1;
    var elem = document.getElementById("myBar");
    var width = 10;
    var id = setInterval(frame, 40);
    function frame() {
      if (width >= 120) {
        clearInterval(id);
        i = 0;
      } else {
        width++;
        if(width>100){
             elem.innerHTML = "It's Infinite";
        }else{
        elem.style.width = width + "%";
        elem.innerHTML = width  + "%";
      }
      }
    }
  }
}
 elem.innerHTML = width  + "%"; 
		
	function startGame() {
	if(x == 100){
			document.getElementById("lol").style.opacity = 1.0 ;
			alert("click the heart icon repeatedly to get your reward");
			x-=10;
		}
		else if (x>50 && x<100) {
		x-=5;
		document.getElementById("lol").style.width = x + "%";
		document.getElementById("lol").style.height = x + "%";
		}else if ( x == 50) {
		alert("You are halfway keep it up");
		x-=2;
		}else if (x>10 && x<50) {
		x-=2;
		document.getElementById("lol").style.width = x + "%";
		document.getElementById("lol").style.height = x + "%";
		}else if ( x == 10) {
		alert("You are too close");
		x-=1;
		}else if (x>0 && x<10 ) {
		x-=1;
		document.getElementById("lol").style.width = x + "%";
		document.getElementById("lol").style.height = x + "%";		
		}else if (x==0) {
			alert("You did it ! here is your prize");
			window.location.href = "https://m.me/100011457304911";
		}
		
	}
	</script>
  </body>

</html>
stackpath.bootstrapcdn.com
