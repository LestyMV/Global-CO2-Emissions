# Global-CO2-Emissions

The dataset we're using will be the first table of this Wikipedia page on carbon dioxide emissions.
Reading in the table as-is will produce a "MultiIndex" dataframe. By renaming all columns you can convert it into a non-MultiIndex dataframe.
Use slicing and/or boolean masks to filter out the rows in this table that aren't countries.

Graph 1: CO2 of the bigger countries
Make a graph of the CO2 emissions of the 5 biggest CO2 producers in the world (based on the latest measurement). The x-axis should be the years of 1990, 2005 and 2017. If newer datapoints are added in the future please include them as well. The y-axis should represent the fossil CO2 emissions in Mt CO2 for the given years. 


Graph 2: worst and best changers
Because of climate change it's important that we curb our carbon dioxide emissions. So some countries will have lowered their emissions while others may have increased their emissions. Some countries will have better results in doing this than others. If we calculate the relative change and sort by that change we'll get a list with countries that are changing for the better at one end and countries that are changing less well on the other end.

Find the top three and bottom three countries with regards to lowering these emissions and plot their results.

Note: If you want to add a new column to a dataframe you can do that like this:
df['example'] = df.loc[:,'column_a'] + df.loc[:,'column_b']

Note: If you need to sort a dataframe by a column use sort_values(opens in a new tab)
The x-axis should have be the years of 1990, 2005 and 2017. If newer datapoints are added in the future please include them as well. The y-axis should represent the relative amount of CO2 emitted where the measurement in 1990 is 100%.

An example: Afghanistan emitted 2546Mt of CO2 in 1990 (which is the 100%). The relative amount in 2005 would be 1063/2546 * 100 = 41.75%. The relative amount in 2017 would be 11.422/2546 * 100 = 448.62%. So if Afghanistan is on the chart the line would go down first and then back up again.

You may get some really small countries if you look at the relative change. This can distort the chart a lot. To create a more useful chart: now create the same chart for all countries that had at least five Mt of CO2 emissions in 1990.
