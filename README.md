# assignment.py
assignment #1 data science 

# Question 1
for i in range(1,10):

   c=i+(i-1)
   print(c)


#    Question 3
numbers = [12, 75, 150, 180, 145, 525, 50]

for number in numbers:
    if number % 5 == 0:
        if number > 500:
            break 
        elif number > 150:
            continue 
        print(number)


# Question 4
a=int(input("enter a number:"))
n1, n2=0, 1
sum = 0
for i in range(0,a):
  print(sum)   
  n1=n2
  n2=sum
  sum=n1+n2


#  Question 5
def fn (n):
    if n==0 or n==1:
        return 1
    else:
        return n*fn(n-1)
c=fn(5)
print(c)


# Question 7
f=[]
a = [3, 6, 9, 12, 15, 18, 21]
b = [4, 8, 12, 16, 20, 24, 28,33]
for c in a :
    if c%2==0:
        f.append(c)
for g in b :
    if g%2!=0:
        f.append(g)

print(f)


# Question 6
sample_list = [11, 45, 8, 11, 23, 45, 23, 45, 89]

# Initialize an empty dictionary to store the count of each element
element_count = {}

# Iterate through the list and count occurrences
for element in sample_list:
    if element in element_count:
        element_count[element] += 1
    else:
        element_count[element] = 1

# Print the count of each element
print("Printing count of each item:", end=" ")
for element, count in element_count.items():
    print(f"{element}: {count}", end=", " if element != list(element_count.keys())[-1] else "")
    
    
    # Question 2
a=5
for i in range(1,a+1):
    for k in range(i):
        print(i, end=" ")
    print()


