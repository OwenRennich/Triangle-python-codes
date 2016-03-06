#! /usr/bin/python

print('Would you like to find a leg or the hypotenuse of your triangle?')
Answer = raw_input ('Leg or Hypotenuse: ')
if Answer == 'Hypotenuse':
	print ('Insert your side values to find the hypotenuse.')
	a = raw_input('Type your first side: ')
	b = raw_input('Type your second side: ')
	a = float(a)
	b = float(b)
	a2 = a ** 2.0
	b2 = b ** 2.0
	print (b2 + a2)**0.5
elif Answer == 'Leg' :
	print ('Insert your side values to find a leg.')
	b = raw_input('Type your known leg: ')
	c = raw_input('Type your hypotenuse: ')
	b = float(b)
	c = float(c)
	b2 = b ** 2.0
	c2 = c ** 2.0
	if b2 > c2:
	 print('You cannot have a leg larger than your hypotenuse, your triangle cannot be a right triangle.')
	 print('Here is your leg IF you mixed up the hypotenuse and leg.')
	 print(b2-c2)**0.5
	else:
	 print(c2 - b2)**0.5
else:
	print('You did not submit a valid answer.')
	print('Please try again.')
	print('moo')
	
