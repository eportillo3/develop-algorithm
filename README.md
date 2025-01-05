<h1>Develop an algorithm</h1>

<h2>Introduction</h2>

An algorithm is a set of steps that can be used to solve a problem. Security analysts develop algorithms to provide the solutions that they need for their work. For example, an analyst may work with users who bring them devices. The analyst may need an algorithm that first checks if a user is approved to access the system and then checks if the device that they have brought is the one assigned to them.

In this lab, you'll develop an algorithm in Python that automates this process.

<h2>Scenario</h2>

In this lab, you're working as a security analyst and you're responsible for developing an algorithm that connects users to their assigned devices. You'll write code that indicates if a user is approved on the system and has brought their assigned device to the security team.

<h3>Task 1</h3>

You'll work with a list of approved usernames along with a list of the approved devices assigned to these users. The elements of the two lists are synchronized. In other words, the user at index 0 in approved_users uses the device at index 0 in approved_devices. Later, this will allow you to verify if the username and device ID entered by a user correspond to each other.

First, to explore how indices in lists work, run the following code cell as is and observe the output. Then, replace each 0 with another index and run the cell to observe what happens.

<img src="https://i.imgur.com/50d1ZSM.png" height="80%" width="80%"/>

<h3>Task 2</h3>

There's a new employee joining the organization, and they need to be provided with a username and device ID. In the following code cell, you are given a username and device ID of this new user, stored in the variables new_user and new_device, respectively. Use the .append() method to add these variables to the approved_users and approved_devices respectively. Afterwards, display the approved_users and approved_devices variables to confirm the added information. Be sure to replace each ### YOUR CODE HERE ### with your own code before you run the following cell.

<img src="https://i.imgur.com/5gyv7ON.png" height="80%" width="80%"/>

<h3>Task 3</h3>

An employee has left the team and should no longer have access to the system. In the following code cell, you are given the username and device ID of the user to be removed, stored in the variables removed_user and removed_device respectively. Use the .remove() method to remove each of these elements from the corresponding list. Afterwards, display both the approved_users and the approved_devices variables to view the removed users. Run the code and observe the results. Be sure to replace each ### YOUR CODE HERE ### with your own code before you run the following cell.

<img src="https://i.imgur.com/y98DI40.png" height="80%" width="80%"/>

<h3>Task 4</h3>

As part of verifying a user's identity in the system, you'll need to check if the user is one of the approved users. Write a conditional statement that verifies if a given username is an element of the list of approved usernames. If it is, display "The user ______ is approved to access the system.". Otherwise, display "The user ______ is not approved to access the system.". Be sure to replace each ### YOUR CODE HERE ### with your own code before you run the following cell.

<img src="https://i.imgur.com/wxwOvvj.png" height="80%" width="80%"/>

<h3>Task 5</h3>

The next part of the algorithm uses the .index() method to find the index of username in the approved_list and store that index in a variable named ind.

When used on a list, the .index() method will return the position of the given value in the list.

Add a statement to display ind in the following code cell to explore the value it contains. Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

<img src="https://i.imgur.com/oEq71bh.png" height="80%" width="80%"/>

<h3>Task 6</h3>

This task will allow you to build your understanding of list operations for the algorithm that you'll eventually build. It will demonstrate how you can find an index in one list and then use this index to display connected information in another list. First, use the .index() method again to find the index of username in the approved_users and store that in a variable named ind. Then, connect ind to the approved_devices and display the device ID located at the index ind. Afterwards, run the cell to observe the result. Be sure to replace each ### YOUR CODE HERE ### with your own code before you run the following cell.

<img src="https://i.imgur.com/rMWBuEg.png" height="80%" width="80%"/>

<h3>Task 7</h3>

Your next step in creating the algorithm is to determine if a username and device ID correspond. To do this, write a conditional that checks if the username is an element of the approved_devices and if the device_id stored at the same index as username matches the device_id entered. You'll use the logical operator and to connect the two conditions. When both conditions evaluate to True, display a message that the username is approved and another message that the user has their assigned device. Be sure to replace each ### YOUR CODE HERE ### with your own code before you run the following cell.

<img src="https://i.imgur.com/rc1i492.png" height="80%" width="80%"/>

<h3>Task 8</h3>

It would also be helpful for users to receive messages when their username is not approved or their device ID is incorrect.

Add to the code by writing an elif statement. This elif statement should run when the username is part of the approved_users but the device_id doesn't match the corresponding device ID in the approved_devices. The statement should also display two messages conveying that information.

Be sure to replace each ### YOUR CODE HERE ### with your own code before you run the following cell.

(After you run the code once with a device_id of "4n482ts", you might want to explore what happens if you assign a different value to device_id.)

<img src="https://i.imgur.com/3wjZinG.png" height="80%" width="80%"/>

<h3>Task 9</h3>

In this task, you'll complete your algorithm by developing a function that uses some of the code you've written in earlier tasks. This will automate the login process.

There are multiple ways to use conditionals to automate the login process. In the following code, a nested conditional is used to achieve the goals of the algorithm. There is a conditional statement inside of another conditional statement. The outer conditional handles the case when the username is approved and the case when username is not approved. The inner conditional, which is placed inside the first if statement, handles the case when the username is approved and the device_id is correct, as well as the case when the username is approved and the device_id is incorrect.

To complete this task, you must define a function named login that takes in two parameters, username and device_id. Afterwards, call the function and pass in different username and device ID combinations to experiment and observe the function's behavior. Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

<img src="https://i.imgur.com/6wSd3BV.png" height="80%" width="80%"/>
