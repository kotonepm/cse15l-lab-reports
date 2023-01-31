# Lab Report 2

## Part 1

**Here is my code for StringServer:**

![Screenshot (38)](https://user-images.githubusercontent.com/103862450/215586307-cb148d5c-83db-4fdc-94f4-9165636043a0.png)

**After adding "/add-message?s=Hello" to the end of the localhost this will show up:**

![Screenshot (37)](https://user-images.githubusercontent.com/103862450/215585355-b991c462-e6f9-46e3-a1b8-8ceb63142c40.png)

When printing "Hello" on the server, the handleRequest method is called. Inside this method, there is a condition statement that checks the path of the URI. Inside the if statement, we see that both the getPath and the equal methods call called on the url. The getPath method returns a string object which contains the path of the given file object and the equals method check if the path is equal to the path we want to find. If our path is only /, then the string "Nick's String" is returned. However, as we see in the else statement both the getPath and the contains method gets called. Again, the getPath returns astring object of the path and the contains method check if there is an "/add-message" in the path. As you can see this is where we check if there is the correct path to add our message. To get the acual word that we want to get, the getQuery method is called so we can get the section after the "?". Next we have a string array called parameters, which takes in the value of the query split by the equal sign. The split method is called so we can split the string at the "=". That leaves the string array, parameters, with the values {"s", "Hello"}. Because we want the word Hello to print out , we want the item at the index 1. We add the item to an empty string with a delimiter at the front so we can enter a new line and return the new updated string (str). 


**After adding "/add-message?s=How are you" to the end of the localhost this will show up:**

![Screenshot (35)](https://user-images.githubusercontent.com/103862450/215585494-a0eebe34-b4cc-4309-81f9-b4f9e1cee415.png)

Printing the message "How are you" in the Server follows exactly the same steps at printing "Hello" on the server. The method handleRequest is still called, which has a conditional statement that checks the path of the url. As stated before, if the getPath equals "/", then the string "Nick's string" returns. However, by using the contains method, we can check if there is an "/add-message" in the path, which is what is required to print a messages in the server. The values in the string array are assigned after the split method is called on the query. However, this time the values are {"s", "How are you"}. Because we want the message "How are you" to print out, we add the item at index 1 to an empty string, add a delimiter for a new line, and return the updated string (str). 

---

## Part 2

**A failure-inducing input for the buggy program**

```
@Test
  public void testReversed() {
    int[] input2 = { 1, 2, 3 };
    assertArrayEquals(new int[]{ 3, 2, 1 }, ArrayExamples.reversed(input2));
  }
```

**An input that doesn’t induce a failure**

```
@Test
  public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
```

**The symptom, as the output of running the tests**

![Screenshot (40)](https://user-images.githubusercontent.com/103862450/215659403-bdebc76f-32e0-4f3a-ad51-5692e4e97f08.png)

**Flawed Code**

```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
```

**Fixed Code**

```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[arr.length - i - 1] = arr[i];
    }
    return newArray;
  }
```

**Why This Fix Works**
* This fix works because the left-hand side and right-hand side assignments are swapped. This is an error because we are essentially assigning arr, the array with values, to the values of newArray, which is an empty list. By assigning the values in arr to newArray, the values are set to the values of an empty list {0, 0, 0}. Furthermore the original array (arr) is returned when we want a newArray. To fix this issue, the first thing is to assign the values of the original array (arr) to the empty array, newArray. This way we set the values of the original arr to the empty array. Lastly, we want to return the empty array with the updated values, so we return newArray. 

---

## Part 3

**Something I learned from lab in week 2 or 3 that you didn’t know before**
* Week 2's activity was very interesting because it opened my eyes to how urls work and how a web server works. Learning about how urls just check for certain numbers and different elements in a url by using if-else conditional statements made me realize that basic java concepts are used to run and idea that is seems complicated. Because websites/web servers are so integrated within my life, I never really thought about how this sites are pull up from the internet. I've definitely taken a closer to the urls of common websites to see if they fall in line with the ideas that we learned during week 2. 

