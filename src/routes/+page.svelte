<head>
	<style>
		:root {
 	  --background: #292929;
  	--white: #ffffff;
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
						transition:  all .2s;
			color: white;
			-webkit-appearance: none;
	font-family: Arial, Helvetica, sans-serif;
	border-radius: 100000px;
	transition:  all .2s;
}
.topnav a:hover {
											box-shadow: 5px 5px 15px #212121, -5px -5px 15px #424242, inset 10px 10px 15px #212121, inset -10px -10px 15px #424242;
}

/* Add a color to the active/current link */
.topnav a.active {
  background-color: var(--selection-blue);
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


	</style>
	
	<title>Home</title>
</head>
<body class="background">
<div class="topnav">
  <a id="1" on:click={() => handleClick("1")} class="active" href="#home">Home</a>
  <a id="2" on:click={() => handleClick("2")} href="#news">News</a>
  <a id="3" on:click={() => handleClick("3")} href="#contact">Contact</a>
  <a id="4" on:click={() => handleClick("4")} href="#about">About</a>
</div>
<div class="div">

<input class="input" bind:value={Name} placeholder="Input Name Here">
<button on:click={Button}>Show {Name}</button>
</div>
</body>


<script>
function Button(){
	alert("You " + Name + "!")
}
let Name = "";

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


	}
}
</script>