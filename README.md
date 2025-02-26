# Hotelmenu
#Define the menu of restaurent
menu={
    'Pasta':40,
    'Pizza':50,
    'Burger':60,
    'salad':80,
    'Coffee':65
}
#Greet the customer
print("Welcome to our restaurent")
#showing the menu
print(" Pasta : 40\nPizza : 50\nBurger : 60\nsalad : 80\nCoffee :65")
no_of_order=int(input("Enter the number of order need to order ="))
order_bill=0
for i in range(no_of_order):
    order=input("Enter the item name to oder :")
    if order in menu:
        order_bill+=menu[order]
        print(f"The item you are ordered is {order}")
    else:
        print("Please enter the item present in the menu")

print(f"The bill amount is {order_bill}")
