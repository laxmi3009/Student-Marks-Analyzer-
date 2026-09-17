# Student-Marks-Analyzer-

# Student Marks Analyzer

name = input("Enter student name: ")

marks = []

n = int(input("Enter number of subjects: "))

for i in range(n):
    mark = float(input(f"Enter marks for subject {i + 1}: "))
    marks.append(mark)

total = sum(marks)
average = total / n

# Grade
if average >= 90:
    grade = "A+"
elif average >= 80:
    grade = "A"
elif average >= 70:
    grade = "B"
elif average >= 60:
    grade = "C"
elif average >= 50:
    grade = "D"
else:
    grade = "F"

print("\n--- STUDENT RESULT ---")
print("Name:", name)
print("Marks:", marks)
print("Total Marks:", total)
print("Average:", average)
print("Highest Marks:", max(marks))
print("Lowest Marks:", min(marks))
print("Grade:", grade)

if average >= 40:
    print("Result: PASS")
else:
    print("Result: FAIL")

