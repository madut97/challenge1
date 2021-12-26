This is my solution for the loan analyzer challenge

## Part 1:Auomate the Calculations Solution:

For part 1.1, I first created a variable called len_loan_costs which stores the length of the loan_costs list, then printed the length of the list in a print f statement. 

For part 1.2, I first created a variable, sum_loans, and then calculated the sum of the loans within the list loan_costs using the sum() function. After storing the sum in this variable, I printed my resulted using a print f statement

For part 1.3, I created a new variable to store the average loan cost, loan_average, and then calculated the average within this variable by dividing sum_loans by len_loan_costs. 

## Part 2:Analyze Loan Data Solution: 

For Part 2.1, in order to analyze loan data and calculate the present value, I first created two variables, future_value and remaining months, and then using the .get() function I assigned the respective values from the loan dictionary. 

For Part 2.2, I first created a new variable, discount_rate, and then stored the given minimum required return value here. After storing the rate, I created another variable, present_value, where I would call all the required variables, future_value, remaining months and discount_rate in order to calculate the present value of the given loan using the values stored in these variables. 

For Part 2.3, I created an if-else statement, where the first line checks whether or not the present value is greater than or equal to the cost, and prints the loan is worth at least the cost if the present value is greater than or equal to the loan cost, or prints a message that the loan is not too expensive if the present value is less than the loan cost.

## Part 3:Perform Financial Calculations Solution:

For Part 3.1, I initially defined a function calculate present value, which takes in 3 perimeters, future_value, remaining_months, annual discount rate. Then, within that function, I created a variable present_value, which uses the values for the 3 provided perimeters and calculates the present value of a loan. Lastly, the function returns the present_value using a return statement. 

For Part 3.2, prior to caculating the preset value of the loan stored in new_loan, I created a varaible to, annual_discount_rate and stored the given return rate here. Then I calculated the present value of the loan by calling the given perimeters, future_value and remaining_months from the provided dictionary and the discount rate from the variable I previously created store the discount rate provided.

## Part 4: Conditionally filter lists of loans

For 4.1, prior to the filtering process, I created an empty list labeled inexpensive_loans to store the inexpensive loans selected during the filtering process. 

For part 4.2, using a for statement, I looped through all the loans in the provided dictionary, and then appended the ones that were less than or equal to 500 to the inexpensive_loans list by using the .appennd() function. Then, using a print statement, I printed all the inexpensive loans stored within this list. 

## Part 5: Save the results

For part 5.1, I initially stored an empty csv file within the challenge folder. 

Then, I created a variable header where the headers to be used would be stored in a list format. 

Thereafter, I created a variale to store the output, output_path, where the empty csv file would be referenced using the Path() functionality from the pathlib library. 
 
For the last part, prior to making the iterations, using with open I opened the csvfile. Then, using the csv.write() functionality, I converted the csv file into a writer format to make the iterations. 

After doing this, using the .writerow() function, I appended the column headers stored within the header variable. 

Finally, using a for loop, I went through the loans stored within the inexpensive_loans list I had created and added them to the csv file, I opened in a write format, by calling the loans using the .values() function, and appending them through the .writerow() function. 















