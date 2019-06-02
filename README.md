# roommate-matching
We match pairs of people according to specified criteria.


We want to match pairs of people according to criteria, assumming unconstrained number of rooms such that if there are n people and k = 2 people per room, the number of rooms would be floor(n/k) if n is even and floor(n/k) + 1 if n is odd. We will place all people into doubles and the remainder in the odd case gets their own room.

# Criteria

1) Gender
What gender are you?
What gender do you want?

2) Subfree
Do you want subfree?

3) First choice
Who do you want to live with (both must agree)?

# Inputs

Out program will take a list of people and their preferences in a csv file. 
(name, gender, preferred gender, subfree?, first choice)

# Output
List of pairs:

name-name

.

.

.

name

In the odd case, there is one person who is in a room by themselves, therefore they are listed by themselves.


# Algorithms ideas

1) List
* Read every entry from input file
* Convert each to object
* Store them in a list
* While list has more than one element 
	* Compute match score between head and every other element in the list and find the element with max match score through linear search
		* match score is weighted (first choice match outweighs all other criteria)
	* Remove the head and the matched elements from the list
		* Sliding 




