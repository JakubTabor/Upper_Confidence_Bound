# Upper_Confidence_Bound
# I am gonna using some math function, so I import math
# First i create my variables, I have 10000 values, so I create N = 10000 and 10 columns, d = 10 it will be useful later
# Then I create empty list for "ads_selected", my "numbers_of_selections" will we a list with a 10 columns, so i multiply it by my variable "d"
# Also my "sums_of_rewards" will be a list multiply by my variable "d", I create variable "total_reward" for future
# Now I make "for loop" from 0 to my N variable so 10000, then I create variable "ad" and "max_upper_bound" variable
# In my "for loop" i create new "for loop" from 0 to my "d" variable, so (10) "if numbers_of_selections of index i is graeater than zero then
# My new variable "average_reward" is "sums_of_rewards of index i / numbers_of_selections of index i"
# Now my variable "delta_i" its from pattern "math.sqrt(3/2 * math.log(n + 1) / numbers_of_selections[i])"
# I create variable "upper_bound" is "average_reward" plus "delta_i"
# Then in "else" i set "upper_bound" at very big value, if my variable will be greater than "max upper bound" it will be equal to this big value
# And my "ad" variable will change into "i"
# When this loop will be running my empty list will be filling with this "ad" "ads_selected.append(ad)"
# My "numbers_of_selections" of index "ad" will be changing of (1) "numbers_of_selections[ad] += 1" 
# Now I create new variable "reward" its values from my dataframe of index "n, ad"
# My "sums_of_rewards of index ad" will be filling with my "reward" "sums_of_rewards[ad] = sums_of_rewards[ad] + reward" 
# And my "total_reward" also will be updated of reward "total_reward = total_reward + reward"
# Finally I plot my results, so "ads_selected" on histogram "plt.hist(ads_selected)"
