# Remove-Multiple-List-in-a-python

# Apporach - 1
# Python program to remove multiple
# elements from a list 

# creating a list
list1 = [11, 5, 17, 18, 23, 50] 
# Iterate each element in list and add them in variable total
for ele in list1:
	if ele % 2 == 0:
		list1.remove(ele)
# printing modified list
print("New list after removing all even numbers: ", list1)

# Apporach-2
# Python program to remove multiple elements from a list 
# creating a list
list1 = [11, 5, 17, 18, 23, 50] 

# will create a new list, 
# excluding all even numbers
list1 = [ elem for elem in list1 if elem % 2 != 0]

print(*list1)

# Apporach-3
# Python program to remove multiple elements from a list 
# creating a list
list1 = [11, 5, 17, 18, 23, 50] 

# given index of elements 
# removes 11, 18, 23
unwanted = [0, 3, 4]

for ele in sorted(unwanted, reverse = True): 
	del list1[ele]

# printing modified list
print (*list)


