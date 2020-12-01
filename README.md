# Unit-13-Carly

Begin by importing or copying your code from Chapter 12 for Carly.

In Chapter 12, you created an interactive StaffWeddingEventDemo class that obtains all the data for a wedding event for Carly's Catering, including details about the event and all the staff members required to work at the event.

In this program, you will be saving the information that you get from the user to a file and then displaying the information from the file.  This is one approach to creating persistent data that can be used again later even after you end a program.

- Create a new file called **EventDemoAndCreateFile.java**
  - You can make this a subclass of EventDemo or copy over the functions needed to get user input for the event number, event type, and number of guests
  - This program will begin by getting the user input for 3 Events and fill an array with these 3 Event objects
  - Rather than displaying the details, you will need to create a method to write the Event data to a file
    - This method should take in an array of Events
    - It will begin by creating a new File to save the data to, such as EventData.txt
      - If the file already exists, you should add on to the existing data
    - You should write the following information to the file for each event:
      - event number, event type code, number of guests, and price
      - Recommend making it comma delimited
      - Avoid including label type information in the file (like "Event number: ") as this grows the file in size unnecessarily.  The user is not expected to ever access the file directly for information

- Create a new file called **DisplayEventFile.java**
  - This program should display the information contained in the data file that the other program makes
    - If the file doesn't exist, it should print out "No Event Data saved yet"
    - If the file does exist, then it should read in each line of data and print the information to the console in a meaningful way (This is when you should include the labels for what each piece of information is)
