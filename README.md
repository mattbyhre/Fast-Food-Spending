# Fast-Food-Spending
This code reveals which region in the U.S. spends the highest average money on fast food.
The table I worked, food regions, contained 3 columns, those being state, region, and fast_food_millions. 
The state column contained U.S. states; the region column had different U.S. regions, West, South, Northeast, and Midwest; and the fast_food_millions column reflects the amount spent for each state with a number given.
To start off my code, from the table, I selected region and then used the average function on the fast_food_millions column and renamed it as average_millions using an alias.
On the next line, I grouped by region. The following line, I ordered by average_millions and added DESC at the end to give me the highest averages first.
With the last line of code, I set a limit of 1 so that I could get just the one region that had the highest average spent in millions.
At first, I had my code set to have it order by fast_food_millions instead of average_millions. This actually gave me the incorrect answer, being the South, because the South had a state, Tennessee, that had a higher number spent than other states. That is why the South showed up at the top from this order by statement.
To fix that issue I ran into, I set order by to average_millions and it gave me the region with the highest average amount spent on fast food, being the West instead of the South.
