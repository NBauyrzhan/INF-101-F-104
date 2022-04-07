# INF-101-F-104
Room for students

my_list = []
n = int(input("Enter the list size    :"))
count = 1
for num in range(n):
    x = float(input("Enter "+str(count)+" element of list:"))
    my_list.append(x)
    count = count + 1
print("Your list:",my_list)

for run in range(n-1):
    for i in range(n-1):
        if my_list[i]>my_list[i+1]:
            my_list[i],my_list[i+1]=my_list[i+1],my_list[i]
print("Bubble sort result:",*my_list)
print("Hello")


my_list = []
n = int(input("Enter the list size:"))
count = 1
for num in range(n):
    x = float(input("Enter "+str(count)+" element of list:"))
    my_list.append(x)
    count = count + 1
print("Your list looks like:",my_list)

for i in range(n - 1):
        m = i
        j = i + 1
        while j < n:
            if my_list[j] < my_list[m]:
                m = j
            j = j + 1
        my_list[i], my_list[m] = my_list[m], my_list[i]
print("Selection sort result:",*my_list)
