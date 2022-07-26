## Pandas Challenge

Analyze Results of Education; examining budgets and testing results of literacy and math across schools, grades, types, budgets, and density.



## Summary

I started by merging the data of two files.  After that I looked back at some of the inquiries we wanted to extract and backed up to the original dataframes separately.

I added to the student dataframe by itself using boolean results for pass/fail columns.

I then went back and combined the datasets again. 

At the time I needed to make summary tables the most, I was struggling to get the correct outup to work because 1. I was still struggling with summary tables, but also, I had used a few different methods of retrieving pass fail columns that were based on dtypes that had another type tied to the result.  For example: I learned that binning the scores into bins of 0-70 and 70-100 can produce a column that says pass or fail, or true or false, however, pass != a string, and True != a boolean, because when binning, you are creating labels.  same with groupby and certain ways of using .loc  Those often result in Int64 as the dtype, but when you look at the result its a "series of Int64"  and cannot be used for future numeric funcions.  

so this is the reason you'll see me hard coding a lot of results the long way.

I pressed forward as far as I could and ran low on time, but this exercise still taught me a lot.  I later improved on manipulating data in pandas to make summary tables, and gained a greater understanding of dictionaries and lists, as well as knowing to watch out for dataframe manipulation tools, potentially giving readable, but unusable results, depending on future plans and operations.

## Team

Special Thanks to both Sanoo Singh and TA Colin for helping me format and further understand .iloc and .loc positioning tools

and Thanks to Sam Espe for taking time to brainstorm ideas for summary tables



