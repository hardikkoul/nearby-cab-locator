# nearby-cab-locator
A c++ project to find cabs in the given proximity of the user.

Given GPS co-ordinates(in degrees) of a person who needs a cab and co-ordinates of all the cabs in the city stored in a text file in JSON format, find the user-id and name of all the cab drivers available in 50 km proximity.

Approach Used:
1. Take latitude and longitude of each cab in and store in JSON encoded input file.
2. Convert latitude and longitude of both, the user and the cab present in degrees to radians.
3. Calculate distance between the user’s location and the cab using Great Circle Distance formula.
5. If distance is found to be less than or equal to 50 kms then output the user-id and name of the cab driver to a new file else take no action.

Procedure to run the program :
1. Save the code and the file customers.json in a same location.
2. Now, compile the code(using cmd : g++ file_name.cpp) and run it(using cmd : ./a.out customer.json) with passing file name customers.json along with proper location.
3. A file named answer.json will be created on the same location where code and customer.json file is existing.
