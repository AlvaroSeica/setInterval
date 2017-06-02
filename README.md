# setInterval()

Kinetic poetry: a list of timers and motion properties

This file is a tentative approach to create a list of timers used in scripting digital kinetic poetry works. 

I invite artists, poets, programmers, critics, and a blend of one of this or more, to modify it, improve it, collaborate.

## Timers

### BASIC

PAUSE statement

    PAUSE <milliseconds>
    PAUSE = <milliseconds> TO <milliseconds>
    
SPEED statement

    SPEED <milliseconds>

Examples: 
Silvestre Pestana's <em>Computer Poetry</em> (1981-83)
bpNichol's <em>First Screening: Computer Poems</em> (1984)
    
    10 PRINT AT 11,6; "COMPUTER POETRY": PAUSE 100
    290 PAUSE 200: PAUSE 200: INK 4: GO TO 60: RUN
    (Pestana 1983)
    
    45  FOR PAUSE = 1 TO 1000: NEXT 
    46  SPEED= 170
    (bpNichol 1984)
    
### ActionScript and JavaScript

setTimeout() and setInterval() methods

    setTimeout(function, milliseconds)
    setInterval(function, milliseconds)
    
clearing methods

    clearTimeout() 
    clearInterval()
    
Examples: 
Stephanie Strickland and Cynthia Lawson Jaramillo’s <em>slippingglimpse</em> (2007)
@ihatch's <em>⌰ [Total Runout]</em> (2015)
@nickmontfort’s <em>Una Página de Babel</em> (2015)
Jörg Piringer’s PHP and JavaScript moveLetterSoup(), animSoup(), lettersoupanim.php (2011)
J.R. Carpenter's JavaScript library word.generator.js in, among others, <em>...and by islands I mean paragraphs</em> abd <em>Notes Very Necessary</em> (2015)

    clearTimeout() 
    var loadingCall:Number = setInterval(preloadSite, 50);
	  (Strickland and Jaramillo 2007: line 4)
    
    setTimeout(grow, (Math.random() * 2400));
    (Hatcher 2015: line 148)
    
    window.setInterval(render, 0);
    (Montfort 2015: line 134)
    
    var init = setInterval("animSoup()", 100);
    (Piringer 2011: line 22)
    
    /**
    * ### Generator.play(Int: interval)
    * Renders and inserts the current frame in its element, and then every interval miliseconds thereafter.
    * 
    * * __interval:__ Interval between generations, in miliseconds.
    */
    Generator.prototype.play = function(interval) {
	    this.stop(); // Stop generator in case it's running.
	    if(interval != null) {
		    this.show();
		    var that = this;
		    this.repeater = setInterval(function(){that.show();}, interval); // Weird stuff to work around scope as detailed here: http://www.vonloesch.de/node/32
		    this.interval = interval;
	    }
	    return this;
      }
    (Carpenter 2013 and 2015: lines 179-184)

    isle1.play(23000); 
	  (Carpenter 2013: line 23)
  
### jQuery

### PHP


## Motion

* Commit often.
* Commit should always contain working code. Do not commit and push half baked code. That might break test and beta.elmcip.net installation and will get reverted from the repository.
* Write informative commit messages. Write why you did the changes, not what you just changed, Git will tell us that.
* Remember to push your changes.

### animate

### Problems importing database
If you are unable to restore (import) the full database, your mysql/mariadb resource settings my be to low. Try upping this to:

     max_allowed_packet = 100M

in your my.cnf or server.cnf  ? WHERE DO I FIND THIS ? and restart the db. server

    mysql.server restart
