# Projects-Me
Projects I built as I learn Python

# This is practice creating a reciept 
# This is a long string for a description
lovely_loveseat_description = '''Lovely Loveseat - Tufted polyester blend on wood. 32 inches high x 40 inches wide x 30 inches deep. Red or white.'''
# creating a price for the loveseat
lovely_loveseat_price = 254.00
# descriptions for a settee
stylish_settee_description = '''Stylish Settee - Faux leather on birch. 29.50 inches high x 54.75 inches wide x 28 inches deep Black.'''
# price for the settee
stylish_settee_price = 180.50
# description for a luxurious lamp
luxurious_lamp_description = '''Luxurious Lamp - Glass and iron. 36 inches tall. Brown with cream shade.'''
# price  for luxurious lamp
luxurious_lamp_price = 52.15
# setting the sales tax value
sales_tax = .088
# Our first customer's purchase
# since they have not purchased anything, the total is zero
customer_one_total = 0
# This is for the list of descriptions of things they purchase. Will add as they make purchases.
customer_one_itemization = ' '
# customer purchases our lovely loveseat!
customer_one_total += lovely_loveseat_price
# adding the purchase description to our itemization list
customer_one_itemization = lovely_loveseat_description
# customer purchased the luxurious lamp as well and we will add to the price
customer_one_total += luxurious_lamp_price
# keeping up with the itemizations by adding the lamp description
customer_one_itemization = lovely_loveseat_description + '''                                         
                                             
                                              ''' + luxurious_lamp_description
# Customer one is ready to check out. Adding sales tax to their total
customer_one_tax = customer_one_total * sales_tax
# Adding their tax to their total
customer_one_total += customer_one_tax
# now starting to print their receipt
print("Customer One Items:")
print(customer_one_itemization)
# adding a couple of spaces to make the end product look cleaner
print("""

""")
#adding customer total and rounding it to the nearest 100th
print("Customer One Total:")
# adding a money sign to make it legit
money_sign = "$"
# rounding the total to the nearest 100th
print(money_sign,round(customer_one_total,2))
# making the generation process more modular without the odd placement of gaps to form the desired look. A.I. assisted.
def generate_receipt(item_descriptions, total_cost):
    print("Customer One Items:")
    print(item_descriptions)
    print("\n")
    print("Customer One Total:")
    print("$", round(total_cost, 2))

# Call the function
generate_receipt(customer_one_itemization, customer_one_total)

