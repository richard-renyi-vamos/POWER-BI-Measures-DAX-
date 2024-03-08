CHATGPT CONVERSATION

-----------

User
create a DAX logical formula for POWER BI that selects a every BLUE item from 1 column AND every CIRCULAR item from column 2 (both conditions should be true)
ChatGPT
To create a DAX logical formula in Power BI that selects every BLUE item from one column and every CIRCULAR item from another column where both conditions are true, you can use the FILTER function in combination with the AND function. Here's how you can do it:

DAX
Copy code
FilteredTable =
FILTER(
    'YourTableName',
    'YourTableName'[Color] = "BLUE" && 'YourTableName'[Shape] = "CIRCULAR"
)
Replace 'YourTableName' with the name of your table, 'Color' with the name of the column containing colors, and 'Shape' with the name of the column containing shapes.

This formula filters the table to only include rows where the color is "BLUE" and the shape is "CIRCULAR". Adjust the column names and values to match your actual data.




