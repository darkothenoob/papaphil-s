# papaphil-s
# a simple pizza ordering program using raw_input and elif statements
order_complete = False
num_pizzas = 0
num_wings = 0
num_drinks = 0
num_deserts = 0
pizza_price = 10
wing_price = 8
desert_price = 5
drink_price = 2
pizza_total = pizza_price * num_pizzas
wing_total = wing_price * num_wings
drink_total = drink_price * num_drinks
desert_total = desert_price * num_deserts
order_total = pizza_total+wing_total+desert_total+drink_total

name = raw_input("Hello! What is your name? ")
print "Hello %s, what would you like to order? " % name

while order_complete == False:
order = raw_input("You can press 1 for Pizza, 2 for Wings, 3 for Desert, 4 for Drinks, or 5 for done ")
if order == “1”:
num_pizzas = raw_input("Ok, how many pizzas would you like to order? ")
print "Ok, you ordered %s pizzas. What else would you like to order? " % num_pizzas
elif order == “2”:
num_wings = raw_input("Ok, how many wings would you like to order? ")
print “Ok, you ordered %s wings, what else would you like to order?” % num_wings
elif order == “3”:
num_deserts = raw_input("Ok, how many deserts would you like to order? ")
print "Ok, you ordered %s deserts, what else would you like to order? " % num_deserts
elif order == “4”:
num_drinks = raw_input(“Ok, how many drinks would you like to order?” )
print "Ok, you ordered %s drinks, what else would you like to order? " % num_drinks
elif order == “5”:
order_complete == True
print “Ok, you ordered %s pizzas, %s wings, %s deserts, %s drinks, bringing your total to %s. Thanks for ordering!” % (str(num_pizzas), str(num_wings), str(num_deserts), str(num_drinks), str(order_total))
