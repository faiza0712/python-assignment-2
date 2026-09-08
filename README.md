# python-assignment-2
1. List Creation
Create age_list with five integers and name_list with five names.

Output note: Both lists will be displayed.


# Create two lists
age_list = [24, 25, 27, 28, 29]
name_list = ['Faiza', 'Anu', 'Priya', 'Divya', 'Kavi']

print('Age List:', age_list)
print('Name List:', name_list)
     
Age List: [24, 25, 27, 28, 29]
Name List: ['Faiza', 'Anu', 'Priya', 'Divya', 'Kavi']
2. List Operations
Complete the following operations in order. Run each cell before moving to the next one.

2.1 Append
append() adds an item at the end of a list.

Output note: Yazhini appears at the end of name_list.


name_list.append('Yazhini')
print('After appending Yazhini:', name_list)
     
After appending Yazhini: ['Faiza', 'Anu', 'Priya', 'Divya', 'Kavi', 'Yazhini']
2.2 Insert
insert(index, value) adds a value at a chosen position.

Output note: 26 is placed at index 2 in age_list.


age_list.insert(2, 26)
print('After inserting 26 at index 2:', age_list)
     
After inserting 26 at index 2: [24, 25, 26, 27, 28, 29]
2.3 Remove
remove() deletes the specified value from a list.

Output note: Yazhini is removed from name_list.


name_list.remove('Yazhini')
print('After removing Yazhini:', name_list)
     
After removing Yazhini: ['Faiza', 'Anu', 'Priya', 'Divya', 'Kavi']
2.4 Pop
pop() removes and returns the last value when no index is given.

Output note: The removed age and the new list are shown.


removed_age = age_list.pop()
print('Removed age:', removed_age)
print('After pop:', age_list)
     
Removed age: 29
After pop: [24, 25, 26, 27, 28]
2.5 Extend
extend() adds several values to a list.

Output note: Three additional ages are added.


age_list.extend([31, 30, 32])
print('After extending age_list:', age_list)
     
After extending age_list: [24, 25, 26, 27, 28, 31, 30, 32]
2.6 Sort in Descending Order
sort(reverse=True) arranges numbers from greatest to smallest.

Output note: The largest age appears first.


age_list.sort(reverse=True)
print('Age List in descending order:', age_list)
     
Age List in descending order: [32, 31, 30, 28, 27, 26, 25, 24]
2.7 Maximum, Minimum and Sum
Use max(), min() and sum() to find values from the final age_list.

Output note: The maximum, minimum and total are displayed.


maximum_age = max(age_list)
minimum_age = min(age_list)
total_age = sum(age_list)

print('Maximum Age:', maximum_age)
print('Minimum Age:', minimum_age)
print('Sum of Ages:', total_age)
     
Maximum Age: 32
Minimum Age: 24
Sum of Ages: 223
3. List Access
Access the first item, last item, items from index 2 to 4, and the list in reverse order. name_list is still available from Step 1.

Output note: Index 2 to 4 uses the slice name_list[2:5] because Python excludes the ending index.


print('First element:', name_list[0])
print('Last element:', name_list[-1])
print('Elements from index 2 to 4:', name_list[2:5])
print('Name List in reverse order:', name_list[::-1])
     
First element: Faiza
Last element: Kavi
Elements from index 2 to 4: ['Priya', 'Divya', 'Kavi']
Name List in reverse order: ['Kavi', 'Divya', 'Priya', 'Anu', 'Faiza']
4. Dictionary Operations
Create a dictionary with five students and their marks.

Output note: A dictionary stores values as key: value pairs.


student_marks = {
    'Faiza': 85,
    'Anu': 76,
    'Priya': 91,
    'Divya': 68,
    'Kavi': 79
}

print('Student Marks:', student_marks)
     
Student Marks: {'Faiza': 85, 'Anu': 76, 'Priya': 91, 'Divya': 68, 'Kavi': 79}
4.1 Access a Mark
Use a student's name (the key) to access the mark.

Output note: Faiza's mark is printed.


print("Faiza's Mark:", student_marks['Faiza'])
     
Faiza's Mark: 85
4.2 Add Janani
Assigning a new key adds a new item to the dictionary.

Output note: Janani is added with mark 80.


student_marks['Janani'] = 80
print('After adding Janani:', student_marks)
     
After adding Janani: {'Faiza': 85, 'Anu': 76, 'Priya': 91, 'Divya': 68, 'Kavi': 79, 'Janani': 80}
4.3 Update a Mark
Assigning a value to an existing key updates that student's mark.

Output note: Anu's mark changes to 82.


student_marks['Anu'] = 82
print("After updating Anu's mark:", student_marks)
     
After updating Anu's mark: {'Faiza': 85, 'Anu': 82, 'Priya': 91, 'Divya': 68, 'Kavi': 79, 'Janani': 80}
4.4 Dictionary Methods
Display the dictionary's keys, values and key-value pairs.

Output note: keys(), values() and items() each display a different view of the dictionary.


print('Keys:', student_marks.keys())
print('Values:', student_marks.values())
print('Items:', student_marks.items())
     
Keys: dict_keys(['Faiza', 'Anu', 'Priya', 'Divya', 'Kavi', 'Janani'])
Values: dict_values([85, 82, 91, 68, 79, 80])
Items: dict_items([('Faiza', 85), ('Anu', 82), ('Priya', 91), ('Divya', 68), ('Kavi', 79), ('Janani', 80)])
5. Set Operations
Create a set containing repeated vowels.

Output note: Sets keep only unique values, so the repeated a and i are removed. The display order of a set may vary.


my_set = {'a', 'e', 'i', 'o', 'u', 'a', 'a', 'i'}
print('My Set:', my_set)
print('Explanation: Sets store unique values, so duplicate a and i values are removed.')
     
My Set: {'u', 'e', 'i', 'a', 'o'}
Explanation: Sets store unique values, so duplicate a and i values are removed.
5.1 Attempt Set Indexing
Try my_set[4]. The error is handled so that the next cells still run.

Output note: A set is unordered and does not support indexing, so Python raises a TypeError.


try:
    print(my_set[4])
except TypeError as error:
    print('Error:', error)
    print('Explanation: Sets are unordered collections and do not support indexing.')
     
Error: 'set' object is not subscriptable
Explanation: Sets are unordered collections and do not support indexing.
5.2 Create set1 and set2
Create the two required sets.

Output note: Set order may vary.


set1 = {1, 3, 5, 7, 9}
set2 = {2, 3, 5, 8, 10}

print('Set 1:', set1)
print('Set 2:', set2)
     
Set 1: {1, 3, 5, 7, 9}
Set 2: {2, 3, 5, 8, 10}
5.3 Union and Intersection
A union contains all unique elements from both sets. An intersection contains only elements common to both sets.

Output note: The intersection is {3, 5}; set order may vary.


union_set = set1.union(set2)
intersection_set = set1.intersection(set2)

print('Union:', union_set)
print('Intersection:', intersection_set)
     
Union: {1, 2, 3, 5, 7, 8, 9, 10}
Intersection: {3, 5}
6. Performance Category
Enter a score from 0 to 10. The program first validates the range, then uses if, elif and else to classify the score.

Above Average: greater than 7
Average: 4 to 7 inclusive
Below Average: less than 4
Output note: Run this cell and type a score such as 7. Try 9, 7, 3, and an invalid value such as 12 separately if you need screenshots for each case.


score = float(input('Enter your score (0 to 10): '))

if score < 0 or score > 10:
    print('Invalid score! Please enter a score between 0 and 10.')
elif score > 7:
    print('Above Average: Excellent performance! Keep up the good work!')
elif score >= 4:
    print("Average: Good effort! Keep practicing, there's room for improvement.")
else:
    print('Below Average: Need to improve your performance; consistent practice will lead to better results.')
     
Enter your score (0 to 10): 10
Above Average: Excellent performance! Keep up the good work!
7. Conclusion
This assignment demonstrated:

List creation, modification, access, sorting and calculations
Dictionary creation, access, addition, update and methods
Set uniqueness, the indexing limitation, union and intersection
User input, range validation, and if/elif/else conditions
All tasks have now been completed.
