# RecallMiner

# 1. Create new macros with the following names:
# - rmmain
# - rmgetore
# - rmrecall
# - rmsupply
# 
# 2. Copy each script into its corresponding macro in uos. 
# 3. Determine a single spot for ore/ingot drop off, and get its xy coordinates. (z is not relevant)
# 4. In the rmmain macro adjust the xy coordinates on line 111 to your specific location
# 5. Mark a rune in this exact location, drop that in a runebook and set it as default. This is your "homebook"
# 6. Have 3 full runebooks of mining spots
# 7. This macro system requires you to have a bonded fire beetle

# How it works:
# This macro will start with rmmain, and will always check to see whether you are "home" or not. It will determine this by
# checking your x/y coordinates to match the above marked spot you set. If we aren't home it will try to mine, unless there are 
# other conditions at play, like full weight, or in range of a red, or don't have a pickaxe etc...
# These conditions will "set a flag" of different sorts and as long as those "flags" are set the macro will try to resolve the issue
# before returning to gather ore. Each trip home the macro will refill supplies as needed.
