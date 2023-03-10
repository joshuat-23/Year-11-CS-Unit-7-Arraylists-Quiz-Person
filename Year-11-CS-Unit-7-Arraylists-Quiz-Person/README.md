# Year-11-CS-Unit-7-Arraylists-Quiz-Person

Ensure that you read all instructions carefully. Do not include any additional methods that are not specified in this quiz description. Think carefully about your solution before coding. Use meaningful variable names and ensure to use proper indentation - take pride in your work! Good luck, have fun! :)

1. Inside the <b>Person</b> class, implement a <b>constructor</b>. The constructor should have three parameters and these parameters should be used to initialize the state of a Person object. 
(1 mark)

2. Inside the <b>Person</b> class, implement <b>getter</b> methods for each of the three properties. 
(1 mark)

3. Inside the <b>Person</b> class, implement <b>setter</b> methods for each of the three properties. 
(1 mark)

4. Inside the <b>Person</b> class, implement a <b>toString</b> method. Your toString method can follow any format so long as it returns a string that consists of all three properties and appropriate whitespaces between them. 
(1 mark)

5. Inside the <b>PersonFactory</b> class, complete the method <b>addPerson</b>. This method will take a <b>Person</b> object and add it to the <b>allPersons</b> list. The <b>Person object will be added to the position in the list corresponding to their last name</b>. That is, the allPersons list will be in ascending alphabetical order according to the last name of the Person objects stored in the allPersons list. (6 marks)

For example:

allPersons = [person1, person2, person3, person4]

person1:
    lastName = “Jacobson”
    
person2:
    lastName = “Jammerson”
    
person3:
    lastName = “Lam”
    
person4:
    lastName = “Monka”
    
Person <b>person5</b> = new Person(“Jacob”, “Lanson”, 19);

addPerson(<b>person5</b>);

allPersons = [person1, person2, person3, <b>person5</b>, person4]

To know which index to insert the person object into in allPersons, you may use the <b>compareTo</b> method in the String class. The <b>compareTo</b> method will return one of three integer values: -1, 0, or +1 depending on the two strings being compared. 

Example:

String str1 = “Lam”;

String str2 = “Lan”;

String str3 = “Lam”;

str1.compareTo(str2); 	    // Will return -1 because Lam is less than Lan (lexicographically).

str2.compareTo(str1);	    // Will return +1 because Lan is greater than Lan (lexicographically).

str1.compareTo(str3); 	    // Will return 0 because Lam and Lam are equivalent strings. 

6. Inside the <b>PersonFactory</b> class, complete the method <b>under18</b>. This method will return a <b>new arraylist</b> containing all the person’s that are under the age of 18. (5 marks)

7. Inside the <b>PersonFactory</b> class, complete the method <b>checkLastName</b>. This method will <b>return a boolean</b> depending on whether the allPersons list contains a person whose last name is equal to the argument (actual parameter) that is passed to the method. (5 marks)
