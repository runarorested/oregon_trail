# Oregon Trail for 8-bit

An analisys and modernization of the educative game Oregon Trail by MECC, and porting to 8-bit BASIC systems, like:
- Sinclair BASIC

## The Historical Oregon Trail

The Oregon Trail was a roughly 2,000-mile (about 3,200 km) overland wagon route that pioneers used from the early 1840s through the late 1860s to travel from jumping-off points in Missouri (like Independence or St. Joseph) to the Willamette Valley in Oregon. It crossed prairies, deserts, rivers, and mountain ranges (including the Rockies via South Pass and the Blue Mountains), passing through present-day Kansas, Nebraska, Wyoming, Idaho, and Oregon.

An estimated 300,000 to 400,000 (some sources say up to 650,000) settlers, farmers, families, missionaries, and others traveled it, especially during peak years in the 1840s–1860s. The journey took 4–6 months and was extremely dangerous — disease (like cholera and dysentery), accidents, river crossings, starvation, weather, and occasional conflicts killed roughly 1 in 10 travelers (at least 20,000 deaths total).

The Oregon Trail holds great historical importance for U.S. history, due it's place during the westward expansion. In 1978/1981 it was designated the Oregon National Historic Trail by the U.S. government/National Park Service, with preserved sites, markers, and interpretive centers.

## The educative game

In 1971, an originally text based version of an educative game called [*The Oregon Trail*](https://en.wikipedia.org/wiki/The_Oregon_Trail_(series)) was created to teach history by [Don Rawitsch](https://www.reddit.com/r/IAmA/comments/43ooqf/i_am_don_rawitsch_a_coinventor_of_the_original/), Bill Heinemann, and Paul Dillenberger . Players led a wagon party west, managing supplies, hunting buffalo, dealing with river crossings, broken wagon wheels, and frequent deaths from sicknes, starvation or exposure ("You have died of dysentery" became a legendary meme).

The game, accompanied by a suite of educative material, became one of the most widely distributed educational games ever (tens of millions of copies), introducing generations of American schoolkids to computers, history, and strategy gaming. It shaped how many Americans first learned about the trail — often nostalgically remembered, though later versions have tried to address criticisms about its portrayal of Native peoples and glorification of settlement.

## History of the game

- *December 3, 1971*: **Oregon Trail v1** published by *Rawitsch*, *Heinemann*, and *Dillenberger*, writen in [HP Time-Shared BASIC](https://en.wikipedia.org/wiki/HP_Time-Shared_BASIC), and running on a [HP 2100 minicomputer](https://en.wikipedia.org/wiki/HP_2100).
- *2 weeks later*: Rawitsch deletes program from computer at end of semester
- *October 1974*: Rawitsch hired by the [Minnesota Educational Computing Consortium (MECC)](https://en.wikipedia.org/wiki/MECC), a state-funded organization that developed educational software.
- *November 1974*: Rawitsch rewrites the original game from a teletype paper copy.
- *1975*: **Oregon Trail v2** published by MECC for statewide timeshare systems, written in *BASIC 3.1* and running on the [CDC Cyber 70/73-26](https://en.wikipedia.org/wiki/CDC_Cyber#Cyber_70_and_170_series).
- *1978*: Rawitsch published the full BASIC source code in the May–June 1978 issue of Creative Computing magazine.
- *1985*: **Oregon Trail v3** published by *Philip Bouchard*, written in *Applesoft BASIC* for *Apple II* with color graphics.
- *1995*: **Oregon Trail II** developed by MECC, published by SoftKey Multimedia.

## About the game itself

The game basically implements a management board game, where the player must part from the city of Independence (Missouri), starting with a limited budget, and managing to reach Oregon City (Oregon) before winter comes in less than 9 months (18 in-game turns, from Monday, March 29, 1847 to Monday, November 22, 1847).

Depending the actions of the player, its ubication, and estimated climate at that ubication and turn/date, the player advances a certain number of miles per turn. The objetive is covering the 2000 miles of the Oregon Trail in that time frame without dying.

The game was written:
1. in dialects of Dartmouth BASIC, without letter casing,
2. without support for floating point variables, using fixed point math to emulate them,
3. allowing only one instruction per line,
4. not using advanced instructions like DATA, using multi target GOTOs depending on variable values instead,
5. to be executed in teletype terminals (TTY), meaning that there are no graphical representation, or keyboard controlled menus.

## About this project

The ideas is:
1. to analyze the game,
2. to port it to a more modern BASIC dialect to run it on PC, one that allows multiple instructions per line using:
3. to refractor it in stages to update the code,
  - simplyfy it using more modern functions,
  - simplyfy it using DATAs for readability
  - prepare it to run in super thin terminals (32 and 40 characters wide)
4. to port it to Sinclair BASIC (Sinclair ZX Spectrum), Locomotive BASIC (Amstrad CPC), and Microsoft BASIC variants (IBM Cassette BASIC, Gee-Whiz BASIC, Commodore BASIC 2.0. MSX BASIC),
5. to add color and graphics support if possible.
    
