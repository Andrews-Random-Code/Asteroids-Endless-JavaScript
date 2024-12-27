## Download:
download "asteroids.html" and run it in your browser of choice.

## Gameplay:
A rough take on the original arcade game, asteroids will repeately spawn around your ship in a frequency that slowly increases. Blast them with your gun and dodge them to rack up your score.

## Controls:
Up Arrow moves forward.
Left and Right Arrows rotate the ship.
Space shoots the gun.

## Editing:
This project is organized to make editing easy enough for individual tinkering. For example, to adjust the ship's max speed find the ship constructor:

    const ship = {
		    	x: canvas.width/2,
                    y: canvas.width/2,
	  	  	orientation: 0, //in degrees to later convert to radians
	  	  	momentumAngle: 0,
	  	  	dx: 0,
  		  	dy: 0,
	  	  	scale: 5,
	  	  	speed: 0,
	  	  	topSpeed: 7,
	  	  	acceleration: 0.07,
	  	  	turnRate: 3,
	  	  	visible: true,
	  	  	lives: 3,
	  	  	deathTimerDuration: 150,
	  	  	deathTimer: 0,
	  	  	invulnerabilityPotential: 300,
	  	  	invulnerabilityCurrent: 0,
	  	  	color: "white",
  	  	};

Then adjust the ships "topSpeed" value to whatever seems fun. For example:

        topSpeed: 20,

## Known issues:
The game currently is built to run on 60hz monitors. Faster refresh rates will increase the game speed. I'll probably fix this eventually. This can be fixed on an per system level by adjusting the speeds of objects as demonstrated in the "Editing section".
