# Title
**Dev:** *NeetuU*   
**Date:** *05.31.2023*

## Structured Error Handling (Try-Except)
When you are programming, you fix your bugs immediately and make sure the code runs smoothly. However, it often happens that other people introduce new bugs when they use your program.

### Raising Custom Errors
Python automatically generates errors based on conditions defined by the Python Runtime. However, you can also "raise" errors based on custom conditions (Listing 13). 

```
# ------------------------------------------------- #
# Title: Listing 13
# Description: A try-catch with manually raised errors
# ChangeLog: (Who, When, What)
# NeetuU,05.01.2023,Created Script
# ------------------------------------------------- #

try:
    new_file_name = input("Enter the name of the file you want to make: ")
    if new_file_name.isnumeric():
        raise Exception('Do not use numbers for the file\'s name')
except Exception as e:
    print("There was a non-specific error!")
    print("Built-In Python error info: ")
    print(e, e.__doc__, type(e), sep='\n')
```
#### Listing 13
![Results of Listing 13](https://github.com/upd-neetu/ITFnd100-Mod07/blob/main/Listing13.png)

Figure 13. The results of Listing 13
