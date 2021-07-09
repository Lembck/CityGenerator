# CityGenerator
Creates a name of a city that doesn't exist but looks believable
To see it run in action for yourself visit llamastampede.com/City

# How it works:

To make believable City names, I determined that:
 - letters should be in their usual proportions (such that t is more common than z)
 - letters should be split into a usual consonant and vowel order (such that a word needs a vowel and a word consisting of only 7 vowels won't be allowed)
 
Started with the most populous 500 cities in the USA
Created the Consonant and Vowel Sequences (Ex: Boston -> Cvccvc.)
 - notice the beginning section, 'C', is capitalized and the ending section, 'c.', has a period
Divided the 500 Cities into parts based on the consonant and vowel splits:
 - Ex: Philadelphia -> Ccvcvcvcccvv -> {Cc : Ph, v : i, c : l, v : a, c : d, v : e, ccc : lph, vv. : ia]
 - Preserves counts

When generating a new city name:
 - A random sequence is chosen
 - Each part in the sequence is randomly chosen from the parts dictionary
 - All word parts are joined together to form the new City name
 - Additionally, prefixes and suffixes like East or Pines are randomly added proportionally

# Examples:

Jeltird (Norwalk)
Borlsbarve (Huntsville)
South Toniwnold (Davenport)
Palapois (Meridian)
Cious Palls Center (Sioux Falls)
Mind Gove Cavi (Salt Lake City)
Toscujoil Valley (Hollywood)
Desturmah City (Henderson)
Chagawong Park (Cleveland)
St. Tollavo Beint (Pompano Beach)
Jithiaman (Vancouver)
Vudgotton (Henderson)
Callekia (Bellevue)
Green Caham (Macon)
Cila Falls (Mesa)
Sproretown Forest (Shreveport)
Ber Hendascate (San Bernardino)
Kistare Fragoun (College Station)
Rich Vey Creek (Palm Bay)
Wovbridge (Nashville)

