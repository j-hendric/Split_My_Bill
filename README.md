**Introduction**
Welcome to SplitMyBill, a Blazor application designed to solve the age-old question: Who's turn is it to pay for coffee? This application is built to assist Bob, Jeremy, and their coworkers at Bertram Labs in determining the fairest way to split the coffee bill based on their preferences and the varying prices of their favorite coffee beverages.

**Features**
- Automatic Calculation: SplitMyBill automatically calculates who should pay for coffee each day based on provided preferences and prices.
- Fair Distribution: The program calculates the probability of each coworker paying based on the cost of their preferred coffee beverage relative to the total cost, ensuring fairness.
- Random Selection: A random number between 0 and 1 is generated to select the coworker who will pay for coffee each day, based on their calculated probability.
- Data History: SplitMyBill includes a data history page that tracks the total cost of coffee orders and the total amount each coworker has paid over time. This allows for long-term fairness as statistically, the total cost of coffee ordered and paid will converge.
- Flexibility: The application allows for dynamic updates such as adding new coworkers, removing coworkers who no longer wish to participate, changing coffee preferences, or updated prices at the coffee shop. This reduces assumptions and ensures the application remains flexible over time.

**Assumptions**
In creating SplitMyBill, the following assumptions were made:
- The coffee payment tradition will be a long-running activity, allowing statistical fairness to emerge over time.
- Tipping tendencies are not considered in the calculation, as tips may vary among individuals and are not included in the total amount spent.

**How to Run Locally**
To run SplitMyBill locally, follow these steps:
1) Clone the Repository: Clone the SplitMyBill repository to your local machine using the following command:

_git clone https://github.com/j-hendric/Split_My_Bill.git_

2) Navigate to the cloned directory:

_cd split-my-bill_

3) Build the solution using the .NET CLI:

_dotnet build_

4) Run the application using the .NET CLI:

_dotnet run_

5) Access the Application: Once the application is running, open your web browser and navigate to http://localhost:5146/ to access SplitMyBill.

**Data Entry**
To customize the preferences and prices for SplitMyBill, you can modify the data directly within the application. Each person has a line on the home page where you can enter their coffee amount. New people can be added using the 'Add Person' button and people can be removed using the [X] button. 
Under the 'Historic Data' tab, you can view the Amount Paid, Total Coffee Costs, Percent Paid, and Percent Coffee Costs for each person who has ever been involved in the coffee run. 
