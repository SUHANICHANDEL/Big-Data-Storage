The Railway Management System is a python program that provides basic functionality to manage train details. It allows users to view existing train details, update train information, and add new trains , delete trains , book tickets , aggregate data and sort all trains  stored in the system. 

Usage : 
When you run the program you have first 2 options : 
For Railway administration: 
(i)View, insert, update, and delete train details. 
(ii)View total number of trains and distinct starting stations. 
(iii)Sort trains based on the number of seats available. 
(iv)Perform advanced aggregation commands to analyze train data. 
(v)Exit the system. 
  
 
For Passengers: 
(i)View all available trains with details. 
(ii)Book tickets for selected trains and specified number of passengers. 
(iii)Exit the system. 
  
 
 
1.Show All Train Details: 
This option allows you to view the details of the trains currently stored in the system. When you select this option, the program will display the train id,train name, its starting station,its destination and no of seats available . If there are no trains in the system, it will inform you that there are no trains to display. 
  
 
2.Add New Train: 
This option allows you to add new trains to the system. Here's how it works: (i) For each train you want to add, you'll be asked to provide the following information: 
      Enter train Id:  
      Enter train name:  
      Enter starting station:  
      Enter destination of train:  
      Enter number of seats present in the train:  
(ii) After entering this information, the program will add the new train to the System. 
  
 
 
3.Update Train Details:  
Choosing this option enables you to update the details of an existing product. Here's how it works. 
(i)	You first need to specify which train you want to update by entering its id. 
(ii)	You can then choose what specific information you want to update. 
(iii)	After selecting what to update, you provide the new information.  If the train with the specified id is not found, the program will notify you that the product doesn't exist. 
  
 
 
 
4.4Delete  Train Details:  
The delete_train() function in the provided code is responsible for deleting a train entry from the database based on the provided train ID. 
(i) The function prompts the user to input the train ID of the train they want to delete. 
(ii)Using the train ID provided by the user, the function performs a database operation to delete the train entry from the collection. It uses the delete_one() method provided by PyMongo to delete the document matching the specified train ID. 
(iii)After successfully deleting the train entry from the database, the function prints a confirmation message indicating that the train has been deleted successfully. 
  
 
5.Showing only limited set of trains:  
When using the railway management system, users may want to view only a certain number of 
trains at a time, especially if the database contains a large number of train entries. The limit_entries() function allows users to specify the maximum number of trains they want to see in the output. 
(i)When prompted with the main menu of the railway management system, users can select the option to view a limited number of trains . 
(ii)	Once the user selects the option, the system prompts the user to input the desired limit. The user can input the maximum number of trains they want to see in the output. 
(iii)	After entering the limit, the system retrieves the specified number of train entries from the database and displays them in a tabular format. Each row represents a train, and the columns display information such as train ID, train name, origin station, destination station, and number of seats available. 
(iv)	If the user wants to see more trains beyond the specified limit, they can choose to view additional trains by running the function again with a different limit. 
  
 
 
6.Showing total number of trains:  
When you want to know how many trains are currently available in our system, you can use the "Total Number of Trains" option. 
(i)The system accesses our database where all train information is stored. 
(ii)It goes through all the records in the database and counts how many trains are there. 
(iii) Once it's done counting, it shows you the total number of trains available. 
  
 
7.Sorting of trains:  
Sorting Trains by Available Seats: 
(i)After selecting the option to sort all trains (8. Sort all trains), the system will display the trains sorted based on the number of available seats in descending order. 
(ii)This means that the trains with the most available seats will appear at the top of the list, making it easier for you to find trains with plenty of seating capacity for your journey. 
  
 
   
  
 
 
 
8.Distinct trains:  
When managing railways, it's important to know the starting stations available for different train routes. The "Distinct Origin Stations" feature allows you to see a list of unique starting stations from which trains depart. 
(i)Choose the option that corresponds to viewing distinct origin stations. This could be numbered, depending on the menu provided. 
(ii)Once selected, the system will gather data from the database and present it in a clear, tabular format. 
(iii) If there are no distinct origin stations available in the database, the system will notify you accordingly. 
 
  
 
 
9.Aggreagate functions:  
Our Railway Management System provides powerful aggregation commands to help you analyze data in various ways. Let's dive into how you can use these commands: 
(i)Total Trains from Each Source: This command gives you the total number of trains originating from each source station. 
  
 
 
  
 
(ii)Total Seats Available in Each Destination: Use this command to find out the total number of seats available at each destination station. 
  
 
(iii)	Grouping by Seat-wise and Counting: Want to see how many trains have a specific number of seats? This command groups trains by the number of seats they offer and counts them accordingly. 
 
  
 
(iv)	Average Seats Available per Route: Discover the average number of seats available per route. This command calculates the average number of seats for trains traveling between each origin and destination pair. 
  
 
(v)	Random Sample of Documents: Sometimes, you may want to take a random sample of data to get a quick overview. This command selects a random sample of documents from the collection. 
  
 
(vi)	Trains with Seats Available Between a Range: To filter trains based on the number of seats available within a specified range. 
  
 
10.Booking tickets:  
Ask the user to enter the starting and destination station for his travel.Then we have to enter the number of passengers for the travel. 
We will get the available trains for the route and we can select the train then. 
Then we have to enter the passengers details also and the tickets will be booked then. 
  
 
 
 
11.EXIT 
