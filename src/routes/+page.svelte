<head>
	<style>
		:root {
 	  --background: #292929;
  	--white: #FFFFFF;
		--selection-blue: #107AB0;
		--hover-grey: #999999;
		}

.topnav {
  background-color: #333;
	display: flex;
  overflow: hidden;
	justify-content: center;
	align-items: center;
	text-align: center;
	border-radius: 10000px;
	min-height: 10vh;
				box-shadow: 10px 10px 15px #212121, -10px -10px 15px #424242, inset 2px 2px 15px #333, inset -2px -2px 15px #333;

}
.topnav a {
				margin: 10px;
  		padding: 20px;

  float: left;
  color: #333;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
				background: #333;
			border-radius: 50px;
			border-width: 5px;
			border-color: #333;
			border-style: solid;

			position:relative;
			box-shadow: 10px 10px 15px #212121, -10px -10px 15px #424242, inset 2px 2px 15px #333, inset -2px -2px 15px #333;
			color: white;
			-webkit-appearance: none;
	font-family: Arial, Helvetica, sans-serif;
	border-radius: 100000px;
	transition:  all .2s ease-in-out;
}
.topnav a:hover {
											box-shadow: 5px 5px 15px #212121, -5px -5px 15px #424242, inset 10px 10px 15px #212121, inset -10px -10px 15px #424242;
}

/* Add a color to the active/current link */
.topnav a.active {
  background-color: var(--selection-blue);
				box-shadow: 7px 7px 15px #212121, -7px -7px 15px #525252, inset 1px 1px 15px #333, inset -1px -1px 15px #333;
  color: white;
}

		.background{
  	  background: var(--background);
    	background-size: 400% 400%;
	    size: 0vh;
		}
		.div{
			display: flex;
  		justify-content: center;
  		align-items: center;
  		text-align: center;
  		min-height: 90vh;
			flex-wrap: wrap;
			margin: 10px;
  		padding: 20px;
		}.topdiv{
			background-color: white;
			align-items: top;
			min-height: 5vh;
		}
		button{
			margin: 10px;
  		padding: 20px;

			background: var(--background);
			border-radius: 50px;
			border-width: 5px;
			border-color: var(--background);
			border-style: solid;
			min-width: 150px;
			min-height: 50px;
			position:relative;
			box-shadow: 10px 10px 15px #212121, -10px -10px 15px #424242, inset 2px 2px 15px var(--background), inset -2px -2px 15px var(--background);
						transition:  all .2s;
			color: white;
			-webkit-appearance: none;

			}
			button:hover{
											box-shadow: 5px 5px 15px #212121, -5px -5px 15px #424242, inset 10px 10px 15px #212121, inset -10px -10px 15px #424242;
			}
			.input{
							margin: 10px;
  		padding: 20px;
			color: white;
			background: var(--background);
			border-radius: 50px;
			border-width: 5px;
			border-color: var(--background);
			border-style: solid;
			min-width: 150px;
			position:relative;
			box-shadow: 10px 10px 15px #212121, -10px -10px 15px #424242, inset 2px 2px 15px var(--background), inset -2px -2px 15px var(--background);
			transition:  all .2s;

			}
			.input:focus{
											box-shadow: 5px 5px 15px #212121, -5px -5px 15px #424242, inset 10px 10px 15px #212121, inset -10px -10px 15px #424242;

			}
			textarea:focus, input:focus{
    outline: none;
}

.homepage{
	margin: 40px 40px;
	display: grid;
	background-color: #333;
  overflow: visible;
	justify-content: center;
	align-items: center;
	text-align: center;
	border-radius: 50px;
	
				box-shadow: 10px 10px 15px #212121, -10px -10px 15px #424242, inset 2px 2px 15px #333, inset -2px -2px 15px #333;
				  animation-name: example;
  animation-duration: 8s;
  animation-iteration-count: infinite;

}
p{
  text-decoration: none;
	padding: 10px 10px;
	color: white;
  font-size: 17px;
	font-family: Arial, Helvetica, sans-serif;
	vertical-align: middle;

}
.bold{
	font-weight: bold;
	font-size: 29px;
	
}
.bmax{
	max-width: 200px;
				margin: 20px 50px;
  		padding: 20px;

  float: left;
  color: #333;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
				background: #333;
			border-radius: 50px;
			border-width: 5px;
			border-color: #333;
			border-style: solid;

			position:relative;
			box-shadow: 10px 10px 15px #212121, -10px -10px 15px #424242, inset 2px 2px 15px #333, inset -2px -2px 15px #333;
			color: white;
			-webkit-appearance: none;
	font-family: Arial, Helvetica, sans-serif;
	border-radius: 100000px;
	transition:  all .2s ease-in-out;

}.bmax:hover{
											box-shadow: 5px 5px 15px #212121, -5px -5px 15px #424242, inset 10px 10px 15px #212121, inset -10px -10px 15px #424242;
			}

.hidden{
	display: none;
}
@keyframes example {
  0%   {background-color: #333;}
  25%  {background-color: #373737;}
  50%  {background-color: #383838;}
  100% {background-color: #333;}
}

	</style>
	
	<title>Home</title>
</head>
<body on:load={load()} class="background">
<div class="topnav">
  <a id="1" on:click={() => handleClick("1")} class="active" href="#home">Home</a>
  <a id="2" on:click={() => handleClick("2")} href="#news">Graphics APIs</a>
  <a id="3" on:click={() => handleClick("3")} href="#contact">Game Engine</a>
  <a id="4" on:click={() => handleClick("4")} href="#about">About</a>
</div>
<div class="pagewrapper">
<div class="homepage" id="home">
	<p class="bold">
	Een game engine maken.
	</p>
	<p>In deze homepage ga ik het hebben over hoe game engines werken, in het tweede tabje laat ik de verschillende graphics APIs zien, in het derde tabje laat ik zien hoe je er eentje programmeert met OPENGL en het vierde tabje is het irritante van game engines</p>
	<p class="bold">Game engines:</p>
	<p>Een game engine is een framework voor game developers om games te maken, het maakt het process van een game maken simpeler en sneller. <br>Alle game engines zorgen er voor dat je niet hoeft te klooien met graphics APIs of audio APIs. Dit zijn beide erg complexe onderwerpen. Je moet veel weten van computers en andere onderwerpen om een game engine te maken.</p>
	<p class="bold">Hoe je er een maakt:</p>
	<p>Eerst moet je een taal kiezen voor je game engine, negen van de tien keer is dit C++, C++ is een efficiente taal die veel controle geeft over alles. Maar dit zorgt er ook voor dat het erg lastig is om te gebruiken. Een game engine kan ook gemaakt worden in C#, een makkelijkere taal maar iets langzamer. <br>Wanneer je een taal gekozen hebt moet je een Graphics API kiezen, je kan ook zonder maar dan ben je 2 jaar bezig met je eigen schrijven. De graphics APIs die je kan gebruiken zijn: DirectX en OpenGL, er zijn er meer maar da word te lang... <br>Hiervan zijn DirectX en OpenGL het populairst. Nadat je een graphics API hebt gekozen kan je gaan programmeren. <br> Eerst maak je een window zodat je het oprect kan zien, dan hook je de functies, render_frame, update_frame, get_input. In deze programmeer je 99%. <br>In render_frame zet je alle functies om het van code naar een plaatje te maken. Hiervoor gebruik je buffers en shaders. Eerst word de vertex buffer gelezen (een collectie van allen polygons en hun data) en dan word dat verandert in een 3d object, daarna worden shaders toegevoegd aan die objecten die de objecten kleur geven. Dan word er een matrix gebruikt die rekent uit wat de camera ziet, en nadat dat allemaal gelukt is, krijg je een plaatje, en dan moet je de foto veranderen op de window en dan heb je een frame succesvol gerenderd. In update_frame word er gerekend wat er met de objecten gedaan moet worden, bijvoorbeeld waar een bal naartoe rolt of dat een driehoek draait. Hier worden ook andere dingen zoals effecten berekend die niet in een shader zitten, Particle FX vooral. get_input word gebruikt voor... input (wow), hier worden toetsenbord en muis acties opgenomen om te bereken wat er dan moet gebeuren, bijvoorbeeld als de speler ESCAPE klikt moet het spel afsluiten, of dat er een menu tevoorschijn komt. <br><br><br>Klik deze knop om naar de volgende pagina te gaan.</p>
	<a href="#news" on:click={() => handleClick("2")} class="bmax">Next Page</a>
</div>
<div class="homepage" id="news">
	<p class="bold">
	Graphics APIs.
	</p>
	<p>
	Een graphics API is een hulpmiddel om met gebruik van video kaarten een scene te renderen.
	<br>
	<br>
	Er zijn veel verschillende graphics APIs en ik ga het hebben over DirectX en OpenGL. 
	</p>
	<p class="bold">
	DirectX:
	</p>
	<p>
	DirectX, gemaakt door Microsoft in September 1995. Waarschijnlijk het meest gebruikte graphics API, omdat het zo veel kan.
	<br>
	De rede waarom het zoveel gebruikt word is omdat het zo makkelijk is en veel functies heeft en het makkelijk op Xbox te zetten is. Microsoft heeft een soort gaming graphics API monopoly.

	<br><br>
	DirectX heeft functies zoals ray tracing en networking ingebouwd waardoor het simpel te gebruiken is. 
	<br>
	hier word het raytracing van DirectX12 uitgelegd: 
	</p>
	<iframe width="560" height="315" src="https://www.youtube.com/embed/yaK1e59-oAA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
	<p class="bold">
	OpenGL:
	</p>
	<p>
	OpenGL vergeleken met DirectX is net iets sneller, en werkt op elk operating system, linux, windows, mac. Maakt niet uit. 
	<br>
	Maar het is wel wat moeilijker te gebruiken dan DirectX, en er zitten geen toevoegingen bij zoals ray tracing of networking. Hierdoor duurt het langer om te gebruiken.
	<br>
	Uitgekomen op 20 junie 1992.
	<br>
	<br>
	Een video die OpenGL uitlegt: 
	</p>
	<iframe width="560" height="315" src="https://www.youtube.com/embed/Z9pnmnckcFs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</div>
<div class="homepage" id="contact">
	<p class="bold">Game Renderer in C# en OpenGL:</p>
	<p>Hier leg ik uit hoe je ongeveer een game renderer kan maken met C# en OpenGL. Nog niet een complete game engine want zo ver ben ik nog niet.</p>
	<p>Eerst maak je een nieuw C# project aan in Visual Studio 2022, en daarna moet je de OpenTK library toevoegen, dat is zeg maar OpenGL voor C#.</p>
	<img src="https://media.discordapp.net/attachments/615823897798901761/1028763135034785792/unknown.png" alt="Source Code, Main."/>
	<p>Hier zie je hoe het project een window aan maakt om te zien, met 800 bij 600 pixels. in window.run word het tevoorschijn gehaald om te bekijken.</p>
	<img src="https://media.discordapp.net/attachments/615823897798901761/1028763248574611576/unknown.png" alt="Source Code, vertices."/>
	<p>Hier boven zie je de vertices, dit is een vierkant. Dit is het enigste dat gemaakt word in dit hele project. Vertices zijn de coordinated om aan OpenGL te vertellen waar alles is.</p>
	<img src="https://media.discordapp.net/attachments/615823897798901761/1028763626686906369/unknown.png" alt="Source Code, loader."/>
	<p class="">Wanneer je dat allemaal gedaan hebt kan je de on render frame functie gebruiken om alles te laten zien. Bij shader.use zie je hoe er een shader met een texture (een soort plaatje)<br> toegevoegd word aan het vierkant. Bij shader.setmatrix zie je hoe alles berekend word om een goeie projectie te krijgen zodat het er normaal uitziet. <br>Bij SwapBuffers worden de buffers veranderd om het actuele plaatje te laten zien.</p>
	<img src="https://media.discordapp.net/attachments/615823897798901761/1028763884200398858/unknown.png?width=479&height=676"alt=""/>
	<p>Op update frame worden inputs berekend. bij var input zie je hoe de actuele toetsenbord knoppen gepakt worden om te gebruiken, deze worden gebruikt voor functies om bijvoorbeeld te bewegen. Dit ziet er ingewikkeld uit maar is eigenlijk een stuk makkelijker dan letterlijk al het andere.</p>
	<p>Als dat allemaal lukt zou je uitendelijk iets zoals dit kunnen krijgen (ik heb heel veel overgeslagen om het simpel te houden):</p>
	<img src ="https://media.discordapp.net/attachments/615823897798901761/1028767359193862144/ezgif-2-6a7b71961d.gif" alt="gif"/>
	<p>Zoals u ziet gaat er veel werk in een klein project dat niet veel doet, ik kan hopelijk binnen 4 weken een werkend project hebben. <i>Hopelijk...</p>
</div>
<div class="homepage" id="about">
<p class="bold">uhhh, wat nu?</p>
<p>ik heb letterlijk geen idee wat ik hier kan doen...</p>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. ofzo<br><br>https://github.com/MartinPrograms/</p>
</div>
</div>
</body>


<script>
function Button(){
	alert("You " + Name + "!")
}
let Name = "";
function load(){
	const homepage = document.getElementById("home");
		homepage.classList.add("hidden");
		const news = document.getElementById("news");
		news.classList.add("hidden");
		const contact = document.getElementById("contact");
		contact.classList.add("hidden");
		const about = document.getElementById("about");
		about.classList.remove("hidden");
		//alert("Deze website heeft wat moeite met tabladen verwisselen, om dit te fixen moet je uitzoomen naar ongeveer 80%. Dit zorgt voor een veel betere ervaring. (control en naar beneden scrollen)")
}
function handleClick(index){
	if(index == 1){
		const elem = document.getElementById('1');
		const elem1 = document.getElementById('2');
		const elem2 = document.getElementById("3");
		const elem3 = document.getElementById('4');
		elem.classList.add("active");
				elem1.classList.remove("active");

		elem2.classList.remove("active");

		elem3.classList.remove("active");

		const homepage = document.getElementById("home");
		homepage.classList.remove("hidden");
		const news = document.getElementById("news");
		news.classList.add("hidden");
		const contact = document.getElementById("contact");
		contact.classList.add("hidden");
		const about = document.getElementById("about");
		about.classList.add("hidden");

		
	}
	if(index == 2){
		const elem = document.getElementById('1');
		const elem1 = document.getElementById('2');
		const elem2 = document.getElementById("3");
		const elem3 = document.getElementById('4');
		elem.classList.remove("active");
				elem1.classList.add("active");

		elem2.classList.remove("active");

		elem3.classList.remove("active");

const homepage = document.getElementById("home");
		homepage.classList.add("hidden");
		const news = document.getElementById("news");
		news.classList.remove("hidden");
		const contact = document.getElementById("contact");
		contact.classList.add("hidden");
		const about = document.getElementById("about");
		about.classList.add("hidden");
	}
	if(index == 3){
		const elem = document.getElementById('1');
		const elem1 = document.getElementById('2');
		const elem2 = document.getElementById("3");
		const elem3 = document.getElementById('4');
		elem.classList.remove("active");
				elem1.classList.remove("active");

		elem2.classList.add("active");

		elem3.classList.remove("active");

const homepage = document.getElementById("home");
		homepage.classList.add("hidden");
		const news = document.getElementById("news");
		news.classList.add("hidden");
		const contact = document.getElementById("contact");
		contact.classList.remove("hidden");
		const about = document.getElementById("about");
		about.classList.add("hidden");
	}
	if(index == 4){
		const elem = document.getElementById('1');
		const elem1 = document.getElementById('2');
		const elem2 = document.getElementById("3");
		const elem3 = document.getElementById('4');
		elem.classList.remove("active");
				elem1.classList.remove("active");

		elem2.classList.remove("active");

		elem3.classList.add("active");

const homepage = document.getElementById("home");
		homepage.classList.add("hidden");
		const news = document.getElementById("news");
		news.classList.add("hidden");
		const contact = document.getElementById("contact");
		contact.classList.add("hidden");
		const about = document.getElementById("about");
		about.classList.remove("hidden");
	}
	
}
</script>