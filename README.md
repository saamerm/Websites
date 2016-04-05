# Websites

#Website 1-Theatre
#HTMl
<!DOCTYPE html>
<html>

<head>
  <title>JS Example</title>
  <!--<script src="js.js">
       
    </script>-->
  <script type="text/javascript">
    //You are writing a web site to sell tickets for a movie theater. You need to present a list of two or more movies. Present a text box for the user to type in the name of the movie they want to see and the number of tickets they want. Each ticket costs $12, when they press "Purchase" echo back the move, ticket count and total amount due. Make it pretty...use the styling we learned about in Visual Studio.
 function substitute() {
            var myValue = document.getElementById('myTextBox').value;
                var myTickets = document.getElementById('myNumber').value;
        
    if (myValue.length == 0 && myTickets.length==0) {
                alert('Please enter a real value in the text box!');
                return;
            }
            var myTitle = document.getElementById('title');
            myTitle.innerHTML = myTickets+" tickets of the movie "+myValue +" will cost you $"+12*myTickets;
        }
  </script>
</head>
<!--<body onload ="alert('Hello WOrld')">-->

<body>
  <div class="wrapper">
  <header><h1>Welcome to the EpicU theatre!</h1></header>
  <article class="main">
  <!--taken from cinemark-->
  <p>How many tickets would you like? </p>
  
  <input type="text" id="myNumber" />
  
  <p>Please enter the name of the movie or choose from the pictures: </p>
  
  <input type="text" id="myTextBox" /><input type="submit" value="Purchase" onclick="substitute()" /></br>
  <p></p>
  <a href="#title">
  <input type="button" class="God" id="myButton1" value="God's Not Dead" name="as" title="df" onclick="movieName1()"/> 
  <input type="button" id="myButton2" class="Superman" value="Batman V Super" name="as" title="df" onclick="movieName2()"/> 
  </a>
    <p id="title"></p>
  </article>
  
 <footer>©2016 EpicU Theatre USA, Inc. Century Theatres, Exigo and Exigo Servers are Exigo brands. “EpicU” is a registered service mark of Exigo USA, Inc.
</footer>
  


	<aside class="aside sidebar" role="complementary">
		<div class="wrapper">
				<div class="zen-resources" id="zen-resources">
				<h3 class="resources">Resources:</h3>
				<ul>
					<li class="view-css">
						<a href="style.css" title="View the source CSS file of the currently-viewed design.">
							View This Design&#8217;s <abbr title="Cascading Style Sheets">CSS</abbr>						</a>
					</li>
					<li class="css-resources">
						<a href="http://www.mezzoblue.com/zengarden/resources/" title="Links to great sites with information on using CSS.">
							<abbr title="Cascading Style Sheets">CSS</abbr> Resources						</a>
					</li>
					<li class="blog">
						<a href="" title="Blog">
							<abbr title="Blog">Blog</abbr>						</a>
					</li>
					<li class="zen-submit">
						<a href="" title="About Us">
							About Us						</a>
					</li>
					<li class="contact">
						<a href="" title="">
							Contact						</a>
					</li>
				</ul>
			</div>
		</div>
	</aside>

  </div>
    </body>

</html>
#CSS

body {
  padding: 2em; 
}
.wrapper {
   display: flex;  
flex-flow: row wrap; 
  font-weight: bold;
  text-align: center;
}
.testing123{background: url('http://www.cinemark.com/media/10519639/showtimes_icon_16_closed_caption.png') no-repeat}
.God{padding-top:160px; background: url('http://www.cinemark.com/media/49417706/small.jpg') no-repeat}
.Superman{padding-top:160px; background: url('http://www.cinemark.com/media/MV006095980000/141569_ac_T.jpg') no-repeat}
.wrapper > * {
  padding: 10px;
  flex: 1 100%;
}
header {
  background: tomato;
}
 .aside { flex: 1 auto; }
 .main    { flex: 7 0px; }
 .aside { order: 1;
  background: gold; } 
  .main    { order: 2;
  text-align: left;
  background: deepskyblue; }
  footer  { order: 3;
  background: lightgreen; }
ul{display:flex;flex-flow:column wrap;}
li{display:flex;}



#Javascript


function movieName1() {
  var myValue = document.getElementById('myButton1').value;
  var myTickets = document.getElementById('myNumber').value;

  if (myValue.length == 0 || myTickets.length == 0) {
    alert('Please enter a real value in the text box!');
    return;
  }
  var myTitle = document.getElementById('title');
  myTitle.innerHTML = "Your movie " + myValue + " with " + myTickets + " tickets will cost you $" + 12 * myTickets;
 
   }
function movieName2() {
  var myValue = document.getElementById('myButton2').value;
  var myTickets = document.getElementById('myNumber').value;

  if (myValue.length == 0 || myTickets.length == 0) {
    alert('Please enter a real value in the text box!');
    return;
  }
  var myTitle = document.getElementById('title');
  myTitle.innerHTML = "Your movie " + myValue + " with " + myTickets + " tickets will cost you $" + 12 * myTickets;
 
   }
