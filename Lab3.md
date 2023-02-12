# Lab Report 3

# The command ```grep```

## ```grep -nr```

I found this command-line option by typing "what are some interesting commands for grep within a directory" in ChatGPT, and ChatGPT gives me one of this commands!

**Example 1:** 

The command: ```grep -nr "Lucayans"```

The output:
```
./written_2/travel_guides/berlitz2/Bahamas-History.txt:6:Centuries before the arrival of Columbus, 
a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Origina
lly from South America, they had traveled up through the Caribbean islands, surviving by cultivating 
modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle 
people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Sal
vador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called 
these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the 
Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed
for only two weeks before sailing towards Cuba.
./written_2/travel_guides/berlitz2/Bahamas-History.txt:7:The Spaniards never bothered to settle in the
Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipe
lago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explo
rers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the 
supplies of water on their ships before they began the long journey back to Europe with their cargoes of
South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were 
removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on 
Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.
```
This command-line searches for the string "Lucayans" in all files from *./written_2*. More importantly, it not only 
shows the file's name that contains "Lucayans" which is *Bahamas-History.txt*, but it also exhibits the line number that
contains "Lucayans" in *Bahamas-History.txt* which is line 6 and line 7 and displays the content in those two specific lines.
```grep -nr``` is very useful becuase the users can easily find the specific contents and details about the location of 
"string", such as file name, line number, and its content, by simply using this command instead of looking for all the files. 

**Example 2:** 

The command: ```grep -nr "happiest"```

The output:
```
 ./written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt:151:They call it the “happiest place on earth,” which may
be why more visitors now come here than to any other single attraction anywhere. Surprisingly, four of every
five are adults. Disney World is styled as the most complete vacation destination in existence, offering
sports, nightlife, sightseeing, shopping, camping, hotels, and restaurants all connected by an extensive,
easy-to-use transportation network.
```
This command-line searches for the string "happiest" in all files from *./written_2*. More importantly, it not only 
shows the file's name that contains "happiest" which is *Bahamas-WhereToGo.txt*, but it also exhibits the line number that
contains "happiest" in *Bahamas-WhereToGo.txt* which is line 151 and displays the content in this specific line.
```grep -nr``` is very useful becuase the users can easily find the specific contents and details about the location of 
"string", such as file name, line number, and its content, by simply using this command instead of looking for all the files. 

## ```grep -c```

I found this command-line option by typing "what are some interesting commands for grep within a directory" in ChatGPT, and ChatGPT gives me one of this commands!

**Example 1:** 

The command: ```grep -c "Lucayans" written_2/travel_guides/berlitz2/Bahamas-History.txt```

The output:
```
2
```
This command-line counts the occurence of the string "Lucayans" in the *Bahamas-History.txt* from the given path ```written_2/travel_guides/berlitz2/Bahamas-History.txt```. 
This command's output ```2``` shows the string "Lucayans" occurs 2 times in *Bahamas-History.txt*.
```grep -c``` is very convenient for users becuase they can easily get the occurence of "string" in a specifc file without the need to count the "string" manually in a time-consuming way.

**Example 2:** 

The command: ```grep -c "was" written_2/travel_guides/berlitz2/*.txt```

The output:
```
written_2/travel_guides/berlitz2/Algarve-History.txt:24
written_2/travel_guides/berlitz2/Algarve-Intro.txt:3
written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt:4
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt:32
written_2/travel_guides/berlitz2/Amsterdam-History.txt:20
written_2/travel_guides/berlitz2/Amsterdam-Intro.txt:4
written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt:4
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:57
written_2/travel_guides/berlitz2/Athens-History.txt:27
written_2/travel_guides/berlitz2/Athens-Intro.txt:4
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt:55
written_2/travel_guides/berlitz2/Bahamas-History.txt:17
written_2/travel_guides/berlitz2/Bahamas-Intro.txt:2
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt:32
written_2/travel_guides/berlitz2/Bali-History.txt:19
written_2/travel_guides/berlitz2/Bali-WhatToDo.txt:4
written_2/travel_guides/berlitz2/Bali-WhereToGo.txt:26
written_2/travel_guides/berlitz2/Barcelona-History.txt:17
written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt:48
written_2/travel_guides/berlitz2/Beijing-History.txt:13
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt:35
written_2/travel_guides/berlitz2/Berlin-History.txt:26
written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt:54
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt:35
written_2/travel_guides/berlitz2/Bermuda-history.txt:17
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:46
written_2/travel_guides/berlitz2/Budapest-History.txt:22
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:32
written_2/travel_guides/berlitz2/California-History.txt:29
written_2/travel_guides/berlitz2/California-WhatToDo.txt:0
written_2/travel_guides/berlitz2/California-WhereToGo.txt:29
written_2/travel_guides/berlitz2/Canada-History.txt:47
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:72
written_2/travel_guides/berlitz2/CanaryIslands-History.txt:12
written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt:1
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:23
written_2/travel_guides/berlitz2/Cancun-History.txt:13
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt:35
written_2/travel_guides/berlitz2/China-History.txt:44
written_2/travel_guides/berlitz2/China-WhatToDo.txt:0
written_2/travel_guides/berlitz2/China-WhereToGo.txt:120
written_2/travel_guides/berlitz2/Costa-History.txt:21
written_2/travel_guides/berlitz2/Costa-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt:49
written_2/travel_guides/berlitz2/CostaBlanca-History.txt:15
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Crete-History.txt:18
written_2/travel_guides/berlitz2/Crete-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt:52
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:31
written_2/travel_guides/berlitz2/Cuba-History.txt:12
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt:29
written_2/travel_guides/berlitz2/Nepal-History.txt:12
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt:5
written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt:20
written_2/travel_guides/berlitz2/NewOrleans-History.txt:24
written_2/travel_guides/berlitz2/Paris-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt:46
written_2/travel_guides/berlitz2/Poland-History.txt:15
written_2/travel_guides/berlitz2/Poland-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Portugal-History.txt:18
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt:64
written_2/travel_guides/berlitz2/PuertoRico-History.txt:16
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt:2
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt:38
written_2/travel_guides/berlitz2/Vallarta-History.txt:15
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:11
```
This command-line counts the occurence of the string "was" in all the files from the given path ```written_2/travel_guides/berlitz2/*.txt```. 
This command's output shows all the files from *berlitz2* with the occurence of the string "was" in each file. For example, "was" occurs 11
times in the file *Vallarta-WhereToGo.txt*.
```grep -c``` is very convenient for users becuase they can not only easily get the occurence of "string" in a specifc file without the need to count the "string" manually in a time-consuming way,
but it can also display all the files from the given path along with the occurence of specifc "string" in each file.

## ```grep -A NUMBER```

I found this command-line option by typing "what are some interesting commands for grep within a directory" in ChatGPT, and ChatGPT gives me one of this commands!

**Example 1:** 

The command: ```grep -A 1 "happiest" ./written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt```

The output:
```
They call it the “happiest place on earth,” which may be why more visitors now come here than to any other single attraction anywhere. Surprisingly, four of every five are adults. Disney World is styled as the most complete vacation destination in existence, offering sports, nightlife, sightseeing, shopping, camping, hotels, and restaurants all connected by an extensive, easy-to-use transportation network.
The heart of the complex is the 100-acre (40-hectare) Magic Kingdom, where it’s easy to confuse who’s real and who’s artificial. This is where the park began and where you can meet all your favorite Disney characters — you’ll be able to shake hands with Mickey and get a hug from Goofy. The park has seven sections, including Main Street, USA, with its re-creation of turn-of-the-century America facing the much photographed Cinderella Castle. For a gentle overview of the entire Magic Kingdom, try the aerial tramway at dusk as the lights are coming on.
```
This command-line shows the 1(NUMBER) line after the line where the "happiest" was found from the file *Bahamas-WhereToGo.txt* given by ```./written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt```. It not only exhibits the content of the line that contains "happiest" but also displays the content in ```1``` line after that line which includes "happiest".
```grep -A NUMBER``` is very useful becuase the users can quickly find the specific contents that containing certain "string" with some following contents after that, in which users can read or understand the contents more conveniently and easily. 

**Example 2:** 

The command: ```grep -A 2 "camping" written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt```

The output:
```
In summer locals enjoy an activity called “day camping” which means heading for an open space, erecting a tent, and spending the day relaxing around it — perhaps with a barbecue. At the end of the day, they take the tent down and head home.
Watersports
With so much water around the city, it’s not surprising that water-based sports are very popular. Even on the canals in the city center you’ll find pedalos (sometimes called water cycles) to rent so that you can see the sights on your own steam. Contact them on Tel. 626 5574; fax 624 1033. You can also captain your own boat to explore the area. Canal Motorboats BV has two locations in the city; Tel. 422 7070 for information and reservations.
```
This command-line shows the 2(NUMBER) lines after the line where the "camping" was found from the file *Amsterdam-WhatToDo.txt* given by ```written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt```. It not only exhibits the content of the line that contains "camping" but also displays the content in ```2``` line after that line which includes "camping".
```grep -A NUMBER``` is very useful becuase the users can quickly find the contents that containing certain "string" with some following contents after that, in which users can read or understand the specific contents more conveniently and easily based on how much contents they want to see. 

## ```egrep -i```

I found this command-line option by typing "what are some alternative ways to use grep within a directory" in ChatGPT, and ChatGPT gives me one of this commands!

**Example 1:** 

The command: ```egrep -i "lucayans" ./written_2/travel_guides/berlitz2/Bahamas-History.txt```

The output:
```
Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.
```
This command-line searches the word "lucayans" from the file *Bahamas-History.txt* given by ```./written_2/travel_guides/berlitz2/Bahamas-History.txt```. Even though this file only contains the upper case of the "L" in "Lucayans", but this command will search the string "lucayans" ignoring the case. Therefore, its output will be the contents of two lines that contain "lucayans" no matter the letter case.
```egrep -i``` is very useful becuase the users can find the specific contents that containing certain "string" successfully even with case error, in which users will not be bothered by minor mistake of the case when searching for words. 

**Example 2:** 

The command: ```egrep -i "whatever" ./written_2/non-fiction/OUP/Kauffman/ch10.txt ```

The output:
```
Whatever the risk, two facts are true. First, since the big bang our universe has become enormously complex. Second, we do not have a theory for why the universe is complex. Equally unarguably, the biosphere has increased in molecular diversity over the past four billion years, just as the standing diversity of species has increased. And equally unarguably, the econosphere has become more complex over the past few million years of hominid evolution. We know this with confidence. If we lack a theory, it is not because the staggering facts of increasing diversity and complexity that stare us in the face do not deserve a theory to account for them.
But even after decoherence sets in, geometry is busy all the time trying to build geometry exponentially and everywhere, while simultaneously decohering. Now an interesting feature of the Td/Tr equation alluded to above is that whatever the exponential rate of expansion of geometry may be per Planck time unit, the exponential rate of decoherence, Td, which grows as the mass times the size scale squared of the geometry, increases, until eventually the exponential rate of formation and exponential rate of decoherence of geometry must balance. The exponential expansion of the universe is over. However, linear expansion by construction of geometry can continue. The fastest linear construction of geometry from any tetrahedron would be at the speed of light.
```
This command-line searches the word "whatever" from the file *ch10.txt* given by ```./written_2/non-fiction/OUP/Kauffman/ch10.txt```. Even though this file contains the upper case of the "W" in "Whatever", but this command will search the string "whatever" ignoring the case. Therefore, its output will be the content of lines that has "Whatever" no matter the letter case.
```egrep -i``` is very useful becuase the users can find the specific contents that containing certain "string" successfully even with case error, in which users will not be bothered by minor mistake of the case when searching for words. 

**All these command-line options for ```grep``` are very interesting and useful, in which users can easilly access the information of the contens that include certain "string" from a file or within a direcotry. I personally think it's very cool that ```grep``` can do so many searching and displaying jobs for us, and the only thing we need to do is to type those several letters in the terminal!**
