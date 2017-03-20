# Alchemy Calculator

The ultimate aim of this tool is to allow a user to tick off a list of potencies and provide them with the appropriate mix of reagents in order to produce the desired potion.

The hard part is of course going to be the actual calculation itself.

# Work Notes

## 2017-03-20 22:30

Given two potencies, we should be able to list pairs or triplets of reagents by:

 - shortlisting those reagents which have the selected potencies
 - combining two (or three) reagents to compare potencies
	 - adding the combination to our accepted list if the selected potencies are present in the result

The outcome of this will be a list of potions with resultant potencies, and an updated list of available potencies to select from.

We then display the results.

So a walkthrough:

 - All potencies are listed, no reagents are listed
 - User selects "Unstoppable"
	 - Reagents list is updated to
		 - Blessed Thistle
		 - Blue Entoloma
		 - Bugloss
		 - Butterfly Wing
		 - Columbine
		 - Cornflower
		 - Dragonthorn
		 - Ladyâ€™s Smock
		 - Luminous Russula
		 - Mountain Flower
		 - Namiraâ€™s Rot
		 - Nirnroot
		 - Scrib Jelly
		 - Spider Egg
		 - Torchbug Thorax
		 - Water Hyacinth
		 - Whitecap
		 - Wormwood
	 - Potencies list is updated to
	 	- Detection
		- Invisible
		- Reduce Speed (hindrance)
	 	- Restore Health
	 	- Restore Stamina
	 	- Restore Magicka
	 	- Speed
	 	- Spell Critical
	 	- Unstoppable
	 	- Weapon Critical
	 - Potions list is updated to various products of the available reagents

## 2017-03-20 23:09

Okay, I'm a twit. JavaScript doesn't support associative arrays.

Looks like I'll need to produce mapping arrays from index to name for reagents and potencies, then a table mapping reagents to potencies.

Perhaps I'll end up having to enumerate every potion that can be made. Ick.

Also: do two positive potencies outweigh a negative potency?
