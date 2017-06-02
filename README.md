# setInterval()

Kinetic Poetry: A List of Timers and Motion Properties

This file is a tentative approach to create a list of timer snippets used in scripting digital kinetic poetry works, as well as motion typologies. Will motion typologies be defined by critical discourse, programming languages, and/or animation libraries with their classes and functions?

I invite artists, poets, programmers, critics, and a blend of one of this or more, to modify it, improve it, collaborate.


## Timers>Platforms

### <a href="https://elmcip.net/platformsoftware/basic" target="_blank">BASIC</a>

PAUSE statement

    PAUSE <milliseconds>
    PAUSE = <milliseconds> TO <milliseconds>
    
SPEED statement

    SPEED <milliseconds>

Works

* Silvestre Pestana's <em>Computer Poetry</em> (1981-83)
* bpNichol's <em>First Screening: Computer Poems</em> (1984)

Examples

    10 PRINT AT 11,6; "COMPUTER POETRY": PAUSE 100
    290 PAUSE 200: PAUSE 200: INK 4: GO TO 60: RUN
    (Pestana 1983)
    
    45  FOR PAUSE = 1 TO 1000: NEXT 
    46  SPEED= 170
    (bpNichol 1984)
    
### <a href="https://elmcip.net/platformsoftware/actionscript" target="_blank">ActionScript</a> and <a href="https://elmcip.net/platformsoftware/javascript" target="_blank">JavaScript</a>

setTimeout() and setInterval() methods

    setTimeout(function, milliseconds)
    setInterval(function, milliseconds)
    
clearing methods

    clearTimeout() 
    clearInterval()
    
duration methods

    transition().duration(milliseconds)
    
Works

* Stephanie Strickland and Cynthia Lawson Jaramillo’s <em>slippingglimpse</em> (2007)
* [@ihatch](https://github.com/ihatch)'s <em>⌰ [Total Runout]</em> (2015)
* [@nickmontfort](https://github.com/nickmontfort)'s <em>Una Página de Babel</em> (2015)
* Jörg Piringer’s PHP and JavaScript moveLetterSoup(), animSoup(), lettersoupanim.php (2011)
* J.R. Carpenter's JavaScript library word.generator.js in, among others, <em>...and by islands I mean paragraphs</em> abd <em>Notes Very Necessary</em> (2015)
* [@jhave](https://github.com/jhave)'s TSNE-animator D3.js <em>Sondheim on BDP: Big-Data-Poetry</em> (2016)

Examples

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
    
    var circle = d3.select(this);
    circle.transition().duration(100)
    (Jhave 2016: lines 134-35)
    
### <a href="https://elmcip.net/platformsoftware/java" target="_blank">Java</a> / <a href="https://elmcip.net/platformsoftware/processing" target="_blank">Processing</a>

Create Works and Examples

### <a href="https://elmcip.net/platformsoftware/jquery" target="_blank">jQuery</a>

jQuery $.animate() Method

Works 

Examples

### <a href="https://elmcip.net/platformsoftware/php" target="_blank">PHP</a>

Create Works and Examples

### <a href="https://elmcip.net/platformsoftware/python" target="_blank">Python</a>

Create Works and Examples

### <a href="https://elmcip.net/platformsoftware/ruby" target="_blank">Ruby</a>

Create Works and Examples

### <a href="https://elmcip.net/platformsoftware/perl" target="_blank">Perl</a>

Create Works and Examples

### <a href="https://elmcip.net/platformsoftware/c" target="_blank">C++</a>

Create Works and Examples


## Motion

### Funkhouser's typology (2007)
* collage
* mutation
* projection
* dislocation of sequences
* interaction

### Bootz's typology (2007)
* syntactic programmed animation: algorithmically transformed syntax
* 3D animation
* digital calligram 
* text in movement/kinetic poetry 
* typographic animation.

### Saemmmer's typology (2010)
* 

### Animation

#### CSS transitions 

##### [Animate.css](https://github.com/daneden/animate.css.git)

Classes

* `bounce`
* `flash`
* `pulse`
* `rubberBand`
* `shake`
* `headShake`
* `swing`
* `tada`
* `wobble`
* `jello`
* `bounceIn`
* `bounceInDown`
* `bounceInLeft`
* `bounceInRight`
* `bounceInUp`
* `bounceOut`
* `bounceOutDown`
* `bounceOutLeft`
* `bounceOutRight`
* `bounceOutUp`
* `fadeIn`
* `fadeInDown`
* `fadeInDownBig`
* `fadeInLeft`
* `fadeInLeftBig`
* `fadeInRight`
* `fadeInRightBig`
* `fadeInUp`
* `fadeInUpBig`
* `fadeOut`
* `fadeOutDown`
* `fadeOutDownBig`
* `fadeOutLeft`
* `fadeOutLeftBig`
* `fadeOutRight`
* `fadeOutRightBig`
* `fadeOutUp`
* `fadeOutUpBig`
* `flipInX`
* `flipInY`
* `flipOutX`
* `flipOutY`
* `lightSpeedIn`
* `lightSpeedOut`
* `rotateIn`
* `rotateInDownLeft`
* `rotateInDownRight`
* `rotateInUpLeft`
* `rotateInUpRight`
* `rotateOut`
* `rotateOutDownLeft`
* `rotateOutDownRight`
* `rotateOutUpLeft`
* `rotateOutUpRight`
* `hinge`
* `jackInTheBox`
* `rollIn`
* `rollOut`
* `zoomIn`
* `zoomInDown`
* `zoomInLeft`
* `zoomInRight`
* `zoomInUp`
* `zoomOut`
* `zoomOutDown`
* `zoomOutLeft`
* `zoomOutRight`
* `zoomOutUp`
* `slideInDown`
* `slideInLeft`
* `slideInRight`
* `slideInUp`
* `slideOutDown`
* `slideOutLeft`
* `slideOutRight`
* `slideOutUp`


#### JavaScript and jQuery

##### [Velocity.js](https://github.com/julianshapiro/velocity)

##### [jquery.transit.js](https://github.com/rstacruz/jquery.transit)

##### [jquery.transition.js](https://github.com/louisremi/jquery.transition.js)

##### [D3](https://github.com/d3/d3)


+++++++More+++++
