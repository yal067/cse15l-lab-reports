# Lab Report 3

## The command ```grep```

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
./travel_guides/berlitz2/Bahamas-WhereToGo.txt:151:They call it the “happiest place on earth,” which may
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

The command: ```grep -c "was" written_2/travel_guides/berlitz2/*.txt ```

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
