This code analyzes the factors that can influence the revenue a character can generate in the game, Honkai Star Rail.

To use the code, follow the instructions:
- Have an HSR.csv file in the same folder as the code. The HSR.csv file should be in the same format as the one in the GitHub with all the same column names.
- Run each segment of code in order:
    - The first segment analyzes the numerical factors and how they correlate with the Total Pulls a character would get.
    - The second segment analyzes the categorical factors and how they correlate
    - The third segment puts all the data from the CSV into a SQL database along with a SQL database with statistical values like Pearson Correlation, Spearman Correlation, p-value, R^2, and F-statistic
    - The last segment will ask the user for input of what they would like to do. It will display a menu and the user can choose a correlating number for the selection they want.
          - Add a character: Once selected it will ask the user to manually input data that is the same as what the other characters have. Once added, the code will give confirmation that the character has been added.
          - Remove a character: Type in the name of the character you want to remove from the database
          - Test a character: The user will input some data that doesn't include Total Pulls, # pulled, and estimated revenue. Once all input, the code will simulate what the missing data could be using the information given. It will then print out all the data sorted by Total Pulls from highest to lowest. Once printed, it will also remove the character from the database so it isn't on there permanently.
          - View Sorted Data: Displays another menu that asks the user on what factor they want to use to sort the data and it will then sort the data from highest to lowest based off what is selected.
          - Print CSV: The code creates a .csv file called New_HSR.csv that has the updated data if the user added or removed any characters. This will it can be renamed to be "HSR.csv" and run again in the code want to test with a higher sample size
- Once the user is done, press 6 on the menu for the last segment to exit the code and close the database.


Project Demo Video: https://drive.google.com/file/d/1zS02ckaCol7w50iUEhsmDxPFO23R72mo/view?usp=sharing
