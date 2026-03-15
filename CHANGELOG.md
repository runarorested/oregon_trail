# CHANGELOG

1. Initial setup
	- Creating README, LICENSE, CHANGELOG
	- Adding original versions of Oregon Trail (v1, v2, Chipmunk BASIC port)
	- Setting Chipmunk BASIC port as work base (oregon.bas)

2. Variable renaming and testing
	- Setting up BASIC interpreters for testing.
	- Setting up .gitignore to ignore the interpreters.
	- Renaming variables and testing until no errors found.
	- Redoing REM header.
	- Redoing Variable List, and moving it to line 9900-9990 range.
	
3. Start, Initilization, Instructions, Difficulty
	- Polishing inputs parsing

4. Shooting subroutine changed and fixed. It uses a count in seconds to determinate
how much did it took you to answer. that delay can be between 0 an  9 seconds, less delay the better, a failure counts as worst delay possible (9). That number is used to calculate
how much ammo you spend and how much food you  hunt. As it was, the original Chipmunk BASIC
port let an unnecesary *3600 on the delay, making it either you make in less of a second and get top result, or always get worst results.