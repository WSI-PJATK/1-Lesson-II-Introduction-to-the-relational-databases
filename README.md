# 1-Lesson-II-Introduction-to-the-relational-databases
1 Lesson II – Introduction to the relational databases 15.03.2024 11:45 | Number of chapters: 8  

## New skills  
The goal of this lecture is to explain the problem of storing data, especially within relational databases. This issue will be studied in depth in future semesters during lectures like “Relational Databases” and “Database Systems”. After studying the five following database related lectures student should be able to explain terms like “data”, “information”, “logical database structure”, know the basics of designing the relational database structure and the basics of SQL query syntax.  
  
The first lecture is dedicated to explaining the need of storing data in today’s world and pointing out the currently used technologies and data models.  
  
## Learning outcome  
Student understands the ubiquity of data stored in various ways depending on the technology used,  
Student understands the need of introducing data structure when storing data,  
Student is able to list the database examples from the everyday life,  
Student understands the existence of various data models and can explain in detail at least two of them.  

# Database – what is it?  

The term „database” in the sense of a system for collecting and storing data dates back to the ancient times. People have always strived for recording their knowledge. The main purpose of this activity was the possibility of drawing conclusions on the basis of possessed information. The basic idea of this mechanism hasn’t changed at all.  

Do you see this sign:  

![](https://gakko.pjwstk.edu.pl/public/7164/WSI_3.png)

https://gakko.pjwstk.edu.pl/public/7164/WSI_3.png

Remember where and inform the others.  
All we need to know is:

How to store this information?
How to make it available?
For whom should we make it available?
While the answer on the third question depends mainly on one’s intentions, the answers to the first and the second questions are strictly dependent on the technology at our disposal. Moreover the technology used can influence the data accessibility and therefore the usability of our solution. Hence our conclusion is: the ability to store information and the extent of its accessibility are determined by the technology we use.

How was data stored in ancient times?  
We can say that one of the important aspects of human history was the way of recording and storing data. Only few were known and all of them were determined by the technology available at that stage of human development.  

Ways of storing data archaic from our perspective  

Clay tablets, cuneiform writing – 4 000 BC till 4 century  

![](https://gakko.pjwstk.edu.pl/public/7164/WSI_4.png)
https://gakko.pjwstk.edu.pl/public/7164/WSI_4.png

Papyrus, handwriting – 3 000 BC until the first century

![](https://gakko.pjwstk.edu.pl/public/7164/WSI_5.png)
https://gakko.pjwstk.edu.pl/public/7164/WSI_5.png

Parchment, handwriting and print – 3rd century BC till 17th century  

…and a little closer to our times  
Finally a few modern technologies  
Paper – discovered in China in 8 BC and used until today around the world  

Print – method of duplication of text with a stamp, known for thousands of years. Modern printing is done using a moveable type invented during the medieval times. The zenith of its development falls on the first half of the 20th century.  

First modern printing machine was constructed significantly later (in second half of 19th century) as an aid for handwriting.  

##… and what was the result of storing this data?  
After many years of acquiring and storing data we managed to collect an enormous amount of data.  

Library of Congress – the biggest library in the world. 142 mln of various documents (29 mln of books, 4.8 mln of maps and atlases, 12 mln of photos, 6 mln of microfilms, 3.5 mln of music documents, 0.5 mln of films). Library consists of 856 km of shelfs in three buildings. There are 22 reading rooms, 5 thousands employees (source: Wikipedia).  

And there are so many other, smaller libraries containing a lot of data.  

What’s our conclusion then? We have enormous collections of data recorded using various old, “classical” technologies. This, however leads to serious problems, such as: how can you find the information you need in this enormous data set using the old technologies? Or how can we make sure that the information coming from two different sources is consistent? And finally, how to decide which information is “true” and which is “false”?  

## Computer – revolution in technology  
…of course not only in the data storing technology. And it did not happen overnight.  

Atanasoff-Berry Computer, ABC – machine used for solving linear algebraic equitation. The first machine was built using 270 electron tubes. It used binary numbers and wasn’t programmable. USA 1939.  

Z3 – (relay successor of mechanic Z3) – Germany, 1941 – the computer was able to perform four types of operations and extract the roots from binary numbers, the clock frequency was 5 1/3 Hz, the memory capacity up to 64 words (each consisting of 22 bits ), the program memory consisted of an eight channel punched tape. Only one model was built and it was subsequently destroyed by the Allied forces. It was used for the endurance calculations of wings in the aircraft industry.  

Colossus – Great Britain – the first one was built on 14th of April in 1941. Altogether 11 models were built. It was used for breaking the code of German encryption machine called (Lorenz machine).  

ENIAC – USA 1943 – 1945 (27 tons, 18 000 electron tubes, 140 square meters). It didn’t have operational memory. It was programmed by manipulating switches and cables. Afterwards it also used punched cards.  

As we can see the beginnings weren’t so easy. But what has the computer brought to the technology of storing data? There are two basic technology advancements we should point out:  

The drop in prices of mass storage (tapes, drives, CD) allowed for storing vast amounts of data on very little space and with little cost.  

The ability to search through data in relatively short time.  
  
But along with these possibilities certain challenges appeared. Various data structures were needed for efficient data storage in order to make a full use of the computer. This is the beginning of the databases in the modern meaning.  
  
Control questions  
Do you think that the computer is necessary for storing data?  
Yes  
No  

Did the concept of data storage appear in the second half of the 20th century?  
Yes  
No  

