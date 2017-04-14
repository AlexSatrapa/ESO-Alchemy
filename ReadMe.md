# Alchemy Calculator

The ultimate aim of this tool is to allow a user to tick off a list of potencies and provide them with the appropriate mix of reagents in order to produce the desired potion.

The hard part is of course going to be the actual calculation itself.

Uses the [Vanilla JS](http://vanilla-js.com) framework.

# Design Notes

Given two potencies, we should be able to list pairs or triplets of reagents by:

 - shortlisting those reagents which have the selected potencies
 - combining two (or three) reagents to compare potencies
	 - adding the combination to our accepted list if the selected potencies are present in the result

The outcome of this will be a list of potions with resultant potencies, and an updated list of available potencies to select from.

We then display the results.

