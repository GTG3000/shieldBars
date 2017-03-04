## Shield Bars API

This modding resource for starbound adds ability to display a custom bar over the head of the player using world.sendEntityMessage.

* Adding/Changing a bar :

world.sendEntityMessage(
  playerId,
  "setBar",
  barName,
  barPercentage,
  barColour
)

barName is a unique identifier for your bar. Store it to modify and remove the bar.
barPercentage is a value between 0 and 1.
barColour is a colour in format of {R, G, B, A}. Values from 0 to 255.

* Removing a bar :

world.sendEntityMessage(
	playerId,
	"removeBar",
	barName
)

## Including this API in your mod:

Install this mod alongside yours, add "requires":["shieldBars"] in your .metadata

Copy this mod contents into yours, add "includes":["shieldBars"] in your .metadata

WARNING - changing the overheadBars function in player primary will lead to compatibility issues. Use the messages.
