# ACCOUNT-USERNAME-CREATION-USING-PYTHON-
BASIC OF PYTHON AND USING IT FOR AUTOMATION 
Cyber Security using Python

# this line of code output a string
print("hello, world!")
hello, world!
print("hello, Eric")
hello, Eric
# This is a statement
# that ouput
#sum of numbers
print(2 + 3)
5
# Multiline comment
""" hdjjdhffhjffjjdhffhdj
hddhddjdhfbf
hfhffhfh"""
print("multi-line commnets")
multi-line commnets
Variables are container to store values, it can use number and variable

num1 = 2
num2 = 3
print(num1 + num2)
5
print(num1,  " is an even number")
2  is an even number
age = 25
gift = "chocolate"
price = 33.5
bonus = 6j
print(age, gift, price, bonus)
25 chocolate 33.5 6j
print(type (age))
<class 'int'>
print(type (gift))
<class 'str'>
print(type (price))
<class 'float'>
print(type (bonus))
<class 'complex'>
# can not add int and string
print(5 + "5")

print(5 + 3.5)
8.5
#string concatenation(a string is not a mathematical or logical)
print("5" + "5")
55
#string concatenation(a string is not a mathematical or logical)
print("5+" + "5")
5+5
num3 = 3.5
#print(type(num3))
num4 = int(num3) #casting from float to int
print(type(num4))
<class 'int'>
num5 = "5"
#print(type(num5))

num6 = int(num5) #casting from str to int
print(type(num6))
<class 'int'>
num7 = 5
num8 ="5"
print(num7 + int(num8))
10
a variabe name must start with letter or underscore
2age = 25
print("my age is" + str(age))

# a variabe must start with alphanumeric character
ip_address = "192.168.1.2"
print("the ip address of my server is " + ip_address)
the ip address of my server is 192.168.1.2
#variables are case sensitive
smtp = 25
Smtp = 587
print(smtp, Smtp)
25 587
# variables can not use some python key reserve words
def = python

variables use descriptive variable name
a = "fec5::bg67::6786::ythf"
print(a)

#variables use descriptive variable name
routermacaddr = "fec5::bg67::6786::ythf"
print(routermacaddr)
fec5::bg67::6786::ythf
#Camel-casing
routerMacAddr = "fec5::bg67::6786::ythf"
print(routerMacAddr)
fec5::bg67::6786::ythf
#Pascal-case
RouterMacAddr = "fec5::bg67::6786::ythf"
print(RouterMacAddr)
fec5::bg67::6786::ythf
#Snake-case
router_mac_addr = "fec5::bg67::6786::ythf"
print(router_mac_addr)
fec5::bg67::6786::ythf
#Many values to multiple varibales
ip_addr1, ip_addr2, ip_addr3 = "192.168.1.1", "192.168.1.2", "192.168.1.3"
print(ip_addr1)
192.168.1.1
ip_addr1, ip_addr2 = "192.168.1.1", "192.168.1.2", "192.168.1.3"
print(ip_addr1)

#One value to multiple variables

ip_addr1 = ip_addr2 = ip_addr3 ="192.168.1.1"
print(ip_addr3)
192.168.1.1
Global & Local Variables

# protocol is global variable
protocol = "https"
# def use as a function
def my_network():
  print(protocol + "://google.com")
my_network()
https://google.com
print(protocol)
https
#protocol3 is local variable

# def is call a function
def my_domain():
  protocol3 = "https"
  print(protocol3 + "://google.com")
my_domain()
https://google.com
print(protocol3)

#protocol2 is global variable using as local variable

# def use to creat function
def my_domain():
  global protocol2
  protocol2 = "https"
  print(protocol2 + "://google.com")
my_domain()
https://google.com
print(protocol2)
https
Python Strings: string is like array

alert = "attacks"
print("attacks")
attacks
alert = "attacks"
print(alert[1])
t
# 16 letter
alert = "attacks immnient"
print(alert[0:3])
att
# 16 letter
alert = "attacks immnient"
print(alert[0:8])
attacks 
# 7 letter1
alert = "attacks"
print(len(alert))
7
# 7 letter1
alert = "attacks"
#print(len(alert))
print(alert[0:7])
attacks
# 16 letter
alert = "attacks imminent"
print(len(alert))

16
alert = "IDS with signature 123 has indicated a potential threat"
print(alert)

IDS with signature 123 has indicated a potential threat
print("attacks" in alert)
False
print("threat" in alert)
True
if "attack" in alert:
    print("Attack detected")
else:
    print("No attack detected")
No attack detected
if "threat" in alert or "attack" in alert or "marlicious" in alert:
    print("security incicdent detected")
else:
    print("no security incicdent detected")
security incicdent detected
if "threat" in alert and "attack" in alert and "marlicious" in alert:
    print("security incicdent detected")
else:
    print("no security incicdent detected")
no security incicdent detected
Python Data Types

Python List:

Is ordered
Is index
Is changeable
Allow duplicates
ports = ['22', '80', '443', '25']
print(ports)
['22', '80', '443', '25']
print(type(ports))
<class 'list'>
print(ports[0])
22
print(ports[2])
443
#since len is 4 then - 1
high = len(ports) - 1
print(ports[high])
25
print(high)
3
#is changeable
status =[22, '88', True, 22]
print(status)
[22, '88', True, 22]
print(len(status))
4
# is changeable- replace what is in 3rd status to 23
status[3] = 23
print(status)
[22, '88', True, 23]
scanners = list(('ssh', 'telent', 'smtp'))
print(type(scanners))
<class 'list'>
print(scanners)
['ssh', 'telent', 'smtp']
print(scanners[0:2])
['ssh', 'telent']
print('ssh' in scanners)
True
print('http' in scanners)
False
Adding an item to a list variable

print(ports)
['22', '80', '443', '25']
#Append will add the new item to the end on the list
# insert you can determine where it should be added to
ports.append('8080')
print(ports)
['22', '80', '443', '25', '8080']
ports.append('90')
print(ports)
['22', '80', '443', '25', '8080', '90']
#insert
ports.insert(2, '23')
print(ports)
['22', '80', '23', '443', '25', '8080', '90']
Removing an item from a list

#remove expect to pass the value
ports.remove('25')
print(ports)
['22', '80', '23', '443', '8080', '90']
#pop expect to pass the index
ports.pop(1)
print(ports)
['22', '23', '443', '8080', '90']
#pop without specifying will remove the last value on the list
ports.pop()
print(ports)
['22', '23', '443', '8080']
To Clear a list- but it will still exist in memory

ports.clear()
print(ports)

To delete from memory use Del

del ports
print(ports)

Looping through a list variable

secure_ports = ['22', '443', '80']
print(secure_ports)
['22', '443', '80']
# To loop, you use for
for port in secure_ports:
  print(port)
22
443
80
all_ports = ['22', '21', '443', '53']
print(all_ports)
['22', '21', '443', '53']
# to loop
for port in all_ports:
  print(port)
22
21
443
53
for port in all_ports:
  if port == '21':
    print('insecure port found', port)
  else:
    print('No insecure port found', port)

No insecure port found 22
insecure port found 21
No insecure port found 443
No insecure port found 53
Python Tuples:

Indexed
Ordered
Allow duplicate
Not changeable
#You use round bracket to create tuple
usernames = ('admin', 'user1', 'user2')
print(usernames)
('admin', 'user1', 'user2')
print(type(usernames))
<class 'tuple'>
print(usernames[1])
user1
print(usernames[1:2])
('user1',)
print(usernames[1:3])
('user1', 'user2')
#it allow duplicate
ports = (25, 80, 53, 53)
print(ports)
(25, 80, 53, 53)
#not changeable
ports[0] = 8080
print(ports)

#to change tuple, it should first covert to a list and covert back to tuple
ports
(25, 80, 53, 53)
ports_list = list(ports)
ports_list[0] = 8080
ports = tuple(ports_list)
print(ports)
(8080, 80, 53, 53)
print(type(ports))
<class 'tuple'>
Python Set:

Unordered
Unindexed
Unchangeable
No duplicate
# Unordered
myset = {'192.168.1.1', '192.168.1.2', '192.168.1.3'}
print(myset)
{'192.168.1.1', '192.168.1.2', '192.168.1.3'}

#unordered and unindexed
print(myset[0])

# No duplicate
myset2 = {'192.168.1.1','192.168.1.1', '192.168.1.2','192.168.1.2', '192.168.1.3'}
print(myset2)
{'192.168.1.1', '192.168.1.2', '192.168.1.3'}
#Unchangeable

Python Dictionaries: Are in key-valiue pairs

Indexed
Ordered
Changeable
No duplicate you create dictionaires by using curly brackets or brace {}
userAccount = {
    'username': 'kzar',
    'password': 'passwords123',
}
print(userAccount)
{'username': 'kzar', 'password': 'passwords123'}
print(type(userAccount))
<class 'dict'>
# Indexed and Ordered
print(userAccount['username'])
kazr
print(userAccount.keys())
dict_keys(['username', 'password'])
userAccount1 = {
    'username': 'kzar',
    'password': 'password123',
    'password': 'password124',
}
print(userAccount1)
{'username': 'kzar', 'password': 'password124'}
userAccount1 = {
    'username': 'kzar',
    'username': 'kzar2',
    'password': 'password123',
}
print(userAccount1)
{'username': 'kzar2', 'password': 'password123'}
userAccount1 = {
    'username': 'kzar',
    'username': 'kzar2',
    'username': 'kzar3',
    'username1': 'kzar3',
    'password': 'password123',
}
print(userAccount1)
{'username': 'kzar3', 'username1': 'kzar3', 'password': 'password123'}
#changeable
userAccount['password'] = 'password1234'
print(userAccount)
{'username': 'kzar', 'password': 'password1234'}

Algorithm: data structure and algorithm List: use [X,Y] Tuple: use (X,Y) Set: use {X,Y} Dictionary: use {X:A, Y:B}

"""
List: [X,Y] fruit = [Mango, Orange, Pineapple, WaterMelon]
Tuple: (X,Y)  fruit = (Mango, Orange, Pineapple, WaterMelon)
Set: {X,Y}    numbers = {1,2,3,4,5}
Dictionary: {X:A, Y:B}
"""

"""
This algorithm will enable the IT/Security admin to automatically assign
device_id(s) and usernames using the name(s) of the employee and the year
the employee joined the organization in a COPE or COBO device deployment
models.
"""
device_id = [] #The unique identifier for employee device(s)
usernames = [] #The unique usernames for the employee(s)

#Function to create unique device id
def createUser(firstname, year):
  year = str(year) #cast the year to a string
  user = firstname[0:2] + year[2:] #Getting the 1st two letters of employee name and adding it to last two numbers of year joined.

  #Check if user already exists
  if user in usernames:
    print("Username already exists")
    newUser = input("choose a unique username: ")
    #Checking if a username has been taken
    if newUser in usernames:
      print("Username already taken")
    #Allow one to choose a unique username
    else:
      usernames.append(newUser)
      d_id = firstname[0:2] + year[2:]
      device_id.append(d_id)
      print("The device id for " + firstname + " is " + newUser)
  #It create unique for usernames that doesn;t exist prior
  else:
    usernames.append(user)
    d_id = firstname[0:2] + year[2:]
    device_id.append(d_id)
    print("The device id for " + firstname + " is " + d_id)
createUser("kazim", 2023)
The device id for kazim is ka23
createUser("kazim", 2023)

Username already exists
choose a unique username: ks23
The device id for kazim is ks23
