# nflrandomgenerator
The Almost Totally Random Pairing Generator: NFL Edition
<html><head><title>The Almost Totally Random Pairing Generator - Version: NFL</title>
	<!--
		The RANDOM PAIRING GENERATOR was designed and programmed by the twisted mind 
		of Glowstick Chick (kimota@unspacy.org) Feel free to distribute and modify 
		it as you wish!
		
		It was later reorganized to be more easily updateable by Aaron Bono.  The
		the div tag for formatting makes it easier for the HTML savy to be able 
		to format their own pages.  The Arrays make it easier to add new items to
		the list and then automatically show up.  We also added the phrases to
		spice up what the pairing meant.  You will need both script tag
		sections and the div tag to make it work (you can change the style sheet
		information on the div tag all you want).  The order of these three IS
		IMPORTANT.
	
		Peace and Slashiness,
		Glowstick Chick
	!-->
	<script language="JavaScript">
	<!--
		var names = new Array(
			"Peyton Manning",
"Calvin Johnson", 
"Tom Brady", 
"LeSean McCoy", 
"Drew Brees", 
"Richard Sherman", 
"Jamaal Charles", 
"A.J. Green", 
"Jimmy Graham", 
"Aaron Rodgers", 
"J.J. Watt", 
"Robert Quinn", 
"Marshawn Lynch", 
"Luke Kuechly", 
"Josh Gordon", 
"Earl Thomas", 
"Joe Thomas", 
"Robert Mathis", 
"Russell Wilson", 
"Andre Johnson", 
"Antonio Brown",
"Cam Newton", 
"Dez Bryant", 
"Terrell Suggs", 
"Mario Williams", 
"Andew Luck", 
"Aldon Smith", 
"Phillip Rivers", 
"Brandon Marshall", 
"Darrelle Revis", 
"Larry Fitzgerald", 
"Joe Haden", 
"Ndamukong Suh", 
"Rob Gronkowski", 
"Vincent Jackson", 
"Haloti Ngata", 
"Frank Gore", 
"Geno Atkins", 
"Demaryius Thomas", 
"Eric Berry", 
"Vernon Davis", 
"Greg Hardy", 
"Alshon Jeffery", 
"Marshal Yanda", 
"DeMarcus Ware", 
"Justin Houston", 
"Joe Flacco", 
"DeAndre Levy", 
"Troy Polamalu", 
"DeSean Jackson", 
"Kam Chancellor", 
"Cameron Wake", 
"Jason Peters", 
"Jared Allen", 
"Justin Smith", 
"Nick Foles", 
"Tony Romo", 
"Antrel Rolle", 
"Wes Welker", 
"Tim Jennings", 
"Von Miller", 
"Clay Matthews", 
"Tyron Smith", 
"Aqib Talib", 
"Pierre Garcon", 
"Colin Kaepernick", 
"T.J. Ward", 
"Jordy Nelson", 
"Kiko Alonso", 
"Reggie Bush", 
"DeMarco Murray", 
"Charles Clay", 
"Eddie Lacy", 
"Matt Forte", 
"Ryan Kalil", 
"Brent Grimes", 
"Jason Witten", 
"Cameron Jordan",
"Matthew Stafford", 
"Alex Smith", 
"Eli Manning", 
"Julian Edelman", 
"Danny Amendola", 
"Eric Decker", 
"Matt Prater", 
"Johnny Manziel", 
"Robert Griffin III", 
"Cam Newton", 
"Ryan Tannehill", 
"Geno Smith", 
"Mark Sanchez", 
"Michael Vick", 
"EJ Manuel", 
"Andy Dalton", 
"Ben Roethlisberger",
"Jay Cutler",
"Christian Ponder",
"Jake Locker",
"Ryan Fitzpatrick", 
"Derek Carr", 
"Teddy Bridgewater", 
"Matt Ryan",
"Nick Foles", 
"Sam Bradford",
"Carson Palmer", 
"football", 
"Sammy Watkins", 
"Mike Wallace", 
"Steve Smith Sr.",
"Jordan Cameron", 
"T.Y. Hilton", 
"Victor Cruz",
"Odell Beckham Jr.", 
"Randall Cobb", 
"Greg Jennings", 


			
		);
		
		var phrases = new Array(
			"at a game",
			"cute dog",
			"here first",
			"trust",
			"first on the scene",
			"primary suspect",
			"after midnight",
			"addiction",
			"another textbook situation",
			"anecdotes",
			"all the world",
			"a real date",
			"a very still life",
			"alone together",
			"awkward",
			"appreciated gesture",
			"actions speak louder than words",
			"another side",
			"a long time ago",
			"across open spaces",
			"after work",
			"all that I've got",
			"after a hard day",
			"anything you want",
			"an honest mistake",
			"black roses",
			"behind closed doors",
			"breaking down",
			"breakfast",
			"backseat",
			"beguiled",
			"between a rock and a hard place",
			"beating heart",
			"by the book",
			"break the rules",
			"beginning to end",
			"bad habit",
			"brains",
			"blatantly obvious",
			"backwards",
			"bend over backwards",
			"burn",
			"basement",
			"boss",
			"connivingly",
			"connections",
			"cross",
			"complete abandon",
	         		"curious",
			"coping mechanisms",
			"Chinese food",
			"children",
			"chivalry is dead",
			"curious",
			"compromising position",
			"college",
			"coffee",
			"collision course",
			"confused",
			"communicate",
			"culture shock",
			"dust yourself off",
			"dizzy",
			"dethroned",
			"damaged",
			"downtown",
			"day off",
			"deal",
			"dangerous",
			"do whatever you like",
			"escape",
			"elevators",
			"everything I'm not",
			"friends with benefits",
			"find the truth",
			"face to face",
			"fall",
			"fishy",
			"for love or money",
			"flirtatious",
			"falling apart",
			"friends and lovers",
			"faith",
			"fixing your clothes",
			"five senses",
			"freeze up",
			"feels so right",
			"frogs",
			"fast food",
			"get it done",
			"ghosts",
			"gut instinct",
			"go for it",
			"games",
			"get to the point",
			"hopeless romantic",
			"handcuffs",
			"haltingly",
			"here I stand",
			"hold me close",
			"hold my hands down",
			"help",
			"healthy competition",
			"hear me out",
			"highest priority",
			"here and now",
			"handling it",
			"heartbeats",
			"hurt me",
			"in traffic",
			"I mean it",
			"in bed",
			"in the rain",
			"in the dark",
			"in the shower",
			"in the future",
			"in the past",
			"infatuated",
			"inked",
			"insurance",
			"in the still of the night",
			"in the club",
			"it means he likes you",
			"just breathe",
			"knock on the door",
			"kinda cute",
			"keep my mouth shut",
			"leather",
			"light a cigarette",
			"light it up",
			"looking for privacy",
			"late night",
			"like riding a bike",
			"logical thinking",
			"leaving a reminder",
			"leaving marks",
			"locked in",
			"love notes",
			"lost the remote",
			"missed",
			"multiple options",
			"matter of ethics",
			"my place",
			"mushy stuff",
			"make a move",
			"medicine",
			"messy",
			"mixed metaphors",
			"Milano cookies",
			"never on time",
			"nonsense",
			"no shirt on",
			"no sleep tonight",
			"new beginnings",
			"not your fault",
			"night owl",
			"not by chance",
			"no touching",
			"not by choice",
			"outside",
			"oddly appealing",
			"open adoration",
			"one night stand",
			"on the rebound",
			"open up",
			"on the phone",
			"only a crush",
			"pride",
			"past my shoulder",
			"processing",
			"promiscuous",
			"plans for tonight",
			"pictures in your hand",
			"pager",
			"professional demeanor",
			"puzzle pieces",
			"pleasant surprise",
			"questioning things",
			"questions and answers",
			"running out of time",
			"release me",
			"ring",
			"routine",
			"ride of your life",
			"rooftop",
			"random things",
			"replacement",
			"stay for a while",
			"saints and sinners",
			"sunshine",
			"sit and dream",
			"snowfall",
			"snark",
			"staring into space",
			"sexy",
			"spend the night",
			"scars",
			"skin",
			"sexual harrasment seminar",
			"sleeping in",
			"soapy water",
			"so different",
			"spellbinding",
			"stay by the phone",
			"satisfy me",
			"searching endlessly",
			"signs",
			"safe",
			"searching for clues",
			"sunrise",
			"sunset",
			"summer",
			"trying to explain",
			"the best of me",
			"tangled up",
			"tied up",
			"the ground you walk on",
			"troubled thoughts",
			"technological know-how",
			"try again",
			"those who wait",
			"thoughts of mortality",
			"target practice",
			"the next morning",
			"three simple words",
			"the next morning",
			"twisted",
			"under lock and key",
			"up in the air",
			"unprofessional",
			"under the weather",
			"using logic to justify actions",
			"unwinding",
			"unresolved issues",
			"unique",
			"undercover",
			"unfinished projects",
			"unnecessary complications",
			"unbuttoned",
			"unbelievable",
			"vacation",
			"with flair",
			"watching you",
			"walk for a minute",
			"whole again",
			"wistful",
			"written all over your face",
			"whisper",
			"wistful",
			"your touch"
		
		);
		
		function generatePairing() {
			var pairingPhrase = "";
		
			// First person
			var index1 = Math.floor(Math.random() * names.length);
			pairingPhrase += names[index1] + " / ";
			
			// Second person
			var index2 = index1;
			while (index2 == index1) {
				index2 = Math.floor(Math.random() * names.length);
			}
			pairingPhrase += names[index2] + " / ";
			
			// Now the phrase
			var index3 = Math.floor(Math.random() * phrases.length);
			pairingPhrase += phrases[index3];
			
			document.getElementById("pairingText").innerHTML = pairingPhrase;
		}
	// -->
	</script>
</head>


<body bgcolor="ffffff" link="#e48158" alink="#e48158" vlink="#8c272d">
<center>
<font face="arial" size="5" color="#000000">The Almost Totally Random Pairing Generator</font>
<br><font face="arial" size="4" color="#000000">Version: Criminal Minds</font>
<br><br><a href="index.html">Random Pairing Generator Index</a></small>
<br>
<br>
<br>

<p>
<center>

<DIV ID="pairingText" STYLE="font-size: 12pt; font-weight: bold; font-family: arial; color: #000000;">
</div>

<SCRIPT LANGUAGE="JavaScript">
<!--
	generatePairing();
//-->
</SCRIPT>

<br>
<br>



<br>
<font face="arial" size="1" color="#000000">
</center>
<b>Still not a good enough plot bunny hatcher? <A HREF="javascript:generatePairing();">Try again</A>!</b>
<br>

<br>Original design by
 <a href="mailto:quietgirl@trigun.com">Glowstick Chick</a> <br>(and tweaked by others, including <a href="http://www.livejournal.com/users/docmichelle/">docmichelle</a> - 

her version is <a href="http://shetiger.com/fanfic/pairinggenerator.html" target="_blank">here</a>)</i>
<br>
<p>
This version created by <a href="http://glaciallyslow.tumblr.com" target="new">glaciallyslow</a>, who did this for reasons.
<p>

</font>

</p>
</body>

</html>
