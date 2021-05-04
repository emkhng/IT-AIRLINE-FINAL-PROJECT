# IT-AIRLINE-FINAL-PROJECT
Requirements: You should name you program res_system_[pawprint].py and develop your program according to the requirements listed below.

You are asked to create a menu driven reservation system for Mizzou IT Airlines using Python. The system should have the ability to load and save reservations data. The system should also allow administrators to view a seating chart and see the sales total  after logging into an admin area in your application. The flight can seat up to 50 people. The seats are arranged in 10 rows of 5 seats each.

Upon starting the application should read the reservation.txt file you are provided, create a flight chart and reserve the seats stored in the file. The user is then to be presented with a menu to choose an option they want to execute.

The reservation system should have the following functionality:

Display the options menu.
Create the seating chart and load the reservations saved in the reservation.txt file when the application starts.
Allow administrators to login with a valid credentials (username and password). Credentials are stored in the admins.txt file.
Calculate and return the total sales for the airline.
Print the flight's seating chart.
Reserve a seat on the airline.
Create and print a confirmation code for the user when they successfully reserve a seat. The confirmation code is a string consisting of alternating characters from the passenger's first name and the title of this course (INFOTC1040). For example if the passenger name was Bob the code would be BIoNbFOTC1040. If the name was Kristofferson it would be KIrNiFsOtToCf1f0e4r0son.
Save the reservation in formation the reservation.txt (passenger first name, passenger seat row, passenger seat column, confirmation code).
Seating Costs: You will need a matrix (list of lists) of the seat costs to calculate the total sales for the airline. The following  function will create a 10 x 5 matrix with the costs for each seat. You should use the function your project. ** If needed, you can run the code below and print the matrix to see what is returned.

'''
Function to create a matrix for seating costs using list comprehensions
'''
def get_seating_costs():
    seat_matrix = [[300, 200, 100, 200, 300] for row in range(10)]
    return seat_matrix
Organizing your code: You should attempt to  develop program using modular programming by creating functions to perform the functionality specified in the requirements. This will make your development process much easier by making you code easier to maintain and debug, and will also allow us to assist you better if you need help. You can also use object oriented programming to create your solution and create python objects and classes.

Look at the following Sample output for the program before you begin coding your solution.

Mizzou IT Airlines
----------------------------------

1. Administrator Log-In Portal
2. Make a Reservation
3. Close Application
What would you like to do? 4
ERROR: Not a valid selection! Select 1 or 2 or 3

What would you like to do? 7
ERROR: Not a valid selection! Select 1 or 2 or 3

What would you like to do?: 1

 Administrator Login Portal
---------------------------

Enter Username: dfgdg
Enter Password: yukdgs
Error: Invalid username/password combination

Enter Username: User1
Enter Password: 24680

Printing the Seating Chart...
['O', 'X', 'X', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'X', 'O']
['X', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'X']
['O', 'X', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'X', 'O', 'O']
['O', 'O', 'O', 'O', 'X']

Total Sales: $1900
You are logged out now!

1. Administrator Log-In Portal
2. Make a Reservation
3. Close Application
Choose an option: 2

Make a Reservation
--------------------

Enter Passenger First Name: Leroy
Enter Passenger Last Name: Collins

Printing the Seating Chart...
['O', 'X', 'X', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'X', 'O']
['X', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'X']
['O', 'X', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'X', 'O', 'O']
['O', 'O', 'O', 'O', 'X']

Which row would you like to sit in? 1

Which seat column would you like to sit in? 2

Row:1 Seat:2 is not available. Please choose again.


Which row would you like to sit in? 1

Which seat column would you like to sit in? 3

Row:1 Seat:3 is not available. Please choose again.


Which row would you like to sit in? 2

Which seat column would you like to sit in? 1

Success! Your requested seat: Row:2 Seat:1 has been assigned.


Printing the Flight Map...
['O', 'X', 'X', 'O', 'O']
['X', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'X', 'O']
['X', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'X']
['O', 'X', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'X', 'O', 'O']
['O', 'O', 'O', 'O', 'X']

Congratulations Leroy Collins! Your trip is now booked! Enjoy!
Your confirmation code is: LIeNrFoOyTC1040

1. Administrator Log-In Portal
2. Make a Reservation
3. Close Application
Choose an option: 3

Thank you for choosing Mizzou IT Airlines! Goodbye!
Submission: Submit a zip file named res_system_[pawprint].zip that contains all the files needed to make the project work.

Note: Your program should not crash and so you must implement all error checking necessary to ensure this.
