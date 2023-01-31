# Lab Report 2

## Part 1

**Here is my code for StringServer:**

![Screenshot (38)](https://user-images.githubusercontent.com/103862450/215586307-cb148d5c-83db-4fdc-94f4-9165636043a0.png)

**After adding "/add-message?s=Hello" to the end of the localhost this will show up:**

![Screenshot (37)](https://user-images.githubusercontent.com/103862450/215585355-b991c462-e6f9-46e3-a1b8-8ceb63142c40.png)

When printing "Hello" on the server, the handleRequest method is called. Inside this method, there is a condition statement that checks the path of the URI. Inside the if statement, we see that both the getPath and the equal methods call called on the url. The getPath method returns a string object which contains the path of the given file object and the equals method check if the path is equal to the path we want to find. If our path is only /, then the string "Nick's String" is returned. However, as we see in the else statement both the getPath and the contains method gets called. Again, the getPath returns astring object of the path and the contains method check if there is an "/add-message" in the path. As you can see this is where we check if there is the correct path to add our message. To get the acual word that we want to get, the getQuery method is called so we can get the section after the "?". Next we have a string array called parameters, which takes in the value of the query split by the equal sign. The split method is called so we can split the string at the "=". That leaves the string array, parameters, with the values {"s", "Hello"}. Because we want the tword Hello to print out , we want the item at the index 1. We add the item to an empty string with a delimiter at the front so we can enter a new line and return the new updated string (str). 


**After adding "/add-message?s=How are you" to the end of the localhost this will show up:**

![Screenshot (35)](https://user-images.githubusercontent.com/103862450/215585494-a0eebe34-b4cc-4309-81f9-b4f9e1cee415.png)

//explain things here

---

## Part 2
