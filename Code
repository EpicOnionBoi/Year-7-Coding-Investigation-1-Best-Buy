#The 5 extra functionality things I did were, percentage discounts, supports decimals, compare more than 2 items, shopping list and user-friendly
#My code is run using multiple functions, which are called via the main function
#All of the "if (variable) == "exit":" lines of code mean that it will go back to the main menu if you type "exit"
#All of the "if anotherfunction == "yes":" lines of code mean that if you answer yes, you will be sent to the main menu

def bestbuycalculator():
  currentnumber = 1 #The variable "currentnumber" is equal to 1 (because this is the first product).
  cheappestnumber = 1 #The variable "cheappestnumber" is equal to 1 (because this is the first product and therefore the cheappest so far).
  cost1 = float(input("The cost of the first product is ($): ")) #This asks the user the cost of the first product.
  mass1 = float(input("The mass of the first product is (g): ")) #This asks the user the mass of the first product.
  unitprice1 = cost1/mass1 #This is where the unit price is calculated. The cost is divided by the mass of the product.
  cheappestcost = unitprice1 #The variable "cheappestcost" is equal to the unit price of the first product (because thhis is the first product and therefore the cheappest so far).
  print("The unit price of this product is", unitprice1, "$/g") #Tells the user the unitprice of the first product in $/g.
  continuation = input("Do you have anything other items? (yes/no) ") #Asks the user if they have another product to compare. 
  if continuation == "exit":
    main()
  while continuation == "yes": #While the variable "coninuation" is equal to "yes", the indented code below will run. This allows the user to compare as many products as they want without limits.
    currentnumber += 1 #This adds 1 to the variable "currentnumber" every time this "while" loop is run.
    cost = float(input("The cost of this product is ($): ")) #Asks the user of the cost of the current product.
    mass = float(input("The mass of this product is (g): ")) #Asks the user of the mass of the current product.
    unitprice = cost/mass #Calculates unit price.
    if unitprice < cheappestcost: #If the current unit price is less than the current cheappest cost, 
      cheappestcost = unitprice #It replaces the previous cheappest cost with the current unit price (which is the cheappest cost).
      cheappestnumber = currentnumber #It also replaces the previous cheappest number with the current product number (because it is now the cheappest product).
    print("The unit price of this product is", unitprice, "$/g") #Tells the user the unit price of the current product.
    continuation = input("Do you have any other items? (answer with yes/no) ") #Once again asks the user if they have any other items. The code will go back to line 12 until the answer is no.
    if continuation == "exit":
      main()
  print("The product with best value is product number", cheappestnumber) #Once there are no more products, it informs the user which product has the best value.
  anotherfunction = input("Is there something else I can help you with? (yes/no) ") 
  if anotherfunction == "yes":
    main()
  elif anotherfunction == "exit":
    main()

def discountcalculator():
  whatfunction2 = input("Which discount calculator would you like? (Answer with 'discounted price calculator' or 'percentage discount calculator') ") #Asks the user if they want a discounted price or percentage discount calculator.
  if whatfunction2 == "discounted price calculator": #If you want a discounted price calculator the indented code below will run.
    originalprice = float(input("What is the original price of the product? ($) ")) #Asks the user what the original price of the product is.
    discount = float(input("What percentage is the discount? (%) ")) #Asks the user what percent the discount is.
    amountleft = 100 - discount #Calculates the percent of the price that is left.
    decimaldiscount = amountleft/100 #Converts the percent of the price left into a decimal.
    discountedprice = originalprice*decimaldiscount #Calculates the discounted price of the product by multiplying the original price and the decimal discount together.
    print("Your discounted price is $" + str(discountedprice)) #Tells the user what the discounted price of the product is.
    again = input("Would you like to calculate another discount? (yes/no) ") #Asks if the user wants to do it again.
    if again == "exit":
      main()
    while again == "yes": #A loop that continues to let you calculate discounted price until you don't want to.
      originalprice = float(input("What is the original price of the product? ($) ")) #Asks the user what the original price of the product is.
      discount = float(input("What percentage is the discount? (%) ")) #Asks the user what percent the discount is.
      amountleft = 100 - discount #Calculates the percent of the price that is left.
      decimaldiscount = amountleft/100 #Converts the percent of the price left into a decimal.
      discountedprice = originalprice*decimaldiscount #Calculates the discounted price of the product by multiplying the original price and the decimal discount together.
      print("Your discounted price is $" + str(discountedprice)) #Tells the user what the discounted price of the product is.
      again = input("Would you like to calculate another discount? (yes/no) ") #Once again asks the user if they want to do it again.
      if again == "exit":
        main()
  elif whatfunction2 == "percentage discount calculator": #If you wanted a percentage discount calculator, the indented code below will run.
    pricebeforediscount = float(input("What is the price before discount? ($) ")) #Asks for price before discount
    priceafterdiscount = float(input("What is the price after discount? ($) ")) #Asks for price after discount
    decimalamountleft = priceafterdiscount/pricebeforediscount #Calculates the decimal out of 1 left after the discount.
    decimalamountdiscounted = 1-decimalamountleft #Calculates the decimal out of 1 that was discounted.
    percentagediscount = decimalamountdiscounted*100 #Calculates the percentage discount.
    print("The percentage discount of this product is", str(percentagediscount) + "%") #Tells the user the percentage discount.
    again = input("Would you like to calculate another discount? (yes/no) ") #Asks if the user wants to do it again.
    if again == "exit":
      main()
    while again == "yes": #A loop that continues to let you calculate discounted price until you don't want to.   
      pricebeforediscount = float(input("What is the price before discount? ($) ")) #Asks for price before discount
      priceafterdiscount = float(input("What is the price after discount? ($) ")) #Asks for price after discount
      decimalamountleft = priceafterdiscount/pricebeforediscount #Calculates the decimal out of 1 left after the discount.
      decimalamountdiscounted = 1-decimalamountleft #Calculates the decimal out of 1 that was discounted.
      percentagediscount = decimalamountdiscounted*100 #Calculates the percentage discount.
      print("The percentage discount of this product is", str(percentagediscount) + "%") #Tells the user the percentage discount.
      again = input("Would you like to calculate another discount? (yes/no) ") #Asks if the user wants to do it again.  
      if again == "exit":
        main()     
  elif whatfunction2 == "exit":
    main()
  else:
    print("I do not understand.") #Says "I do not understand" if you say something random
  anotherfunction = input("Is there something else I can help you with? (yes/no) ")
  if anotherfunction == "yes":
    main()
  elif anotherfunction == "exit":
    main()

def tea():
  print("Waiter: *Puts cup of tea on your table*") #Gives you a cup of tea.
  print("Waiter: Please enjoy your tea") #Tells you to enjoy your tea.
  siptea = input("Would you like to drink the tea? (yes/no) ") #Asks you if you want to drink the tea.
  if siptea == "exit":
    main()
  while siptea == "yes": #A loop that continually asks you if you want to drink the tea again until you say no.
    print("You: *Sips tea*")
    siptea = input("Would you like to drink the tea again? (yes/no) ")
    if siptea == "exit":
      main()
  anotherfunction = input("Is there something else I can help you with? (yes/no) ")
  if anotherfunction == "yes":
    main()
  elif anotherfunction == "exit":
    main()

def shoppinglist():
  shoppinglist = [] #Creates an empty list that items will be put into
  shoppingcost = [] #Creates an empty list that item cost will be put into
  itemname = input("What is the name of the product? ") #Asks for the name of the first product
  if itemname == "exit":
    main()
  shoppinglist.append(itemname) #Puts the name of the item at the end of the shopping list
  itemcost = float(input("What is the cost of this item? ($) ")) #Asks for the cost of the first product
  shoppingcost.append(itemcost) #Puts the cost of the item at the end of the item cost list
  moreitems = input("Do you have any more items to add? (yes/no) ") #Asks if you want to add any more items
  if moreitems == "exit":
    main()
  while moreitems == "yes": #A loop that will run the indented code as long as you have more items to add
    itemname = input("What is the name of the product? ") #Indented code does the same things as above
    if itemname == "exit":
      main()
    shoppinglist.append(itemname)
    itemcost = float(input("What is the cost of this item? ($) "))
    shoppingcost.append(itemcost)
    moreitems = input("Do you have any more items to add? (yes/no) ")
    if moreitems == "exit":
      main()
  print ("All the products in your shopping list are:" ) #Tells you all the items in your shopping list
  for e in shoppinglist:
    print(e)
  print ("The total cost of the items in your list are ($):") #Tells you the total cost of the items in your shopping list
  print(sum(shoppingcost))
  anotherfunction = input("Is there something else I can help you with? (yes/no) ")
  if anotherfunction == "yes":
    main()
  elif anotherfunction == "exit":
    main()

def main():
  print("Hello there, welcome to the best code that you will ever find. Please note that you need to answer everything in lower case.")
  print("If you want to quit, answer 'exit' to any input question that isn't meant to be a number and you will be sent to the main menu.")
  whatfunction = input("To start off, please select a function for me to perform (Choose from best buy calculator, discount calculator, shopping list or tea) ")
  if whatfunction == "best buy calculator": #If you want a best buy calculator, the bestbuycalculator function will run
    bestbuycalculator()
  elif whatfunction == "discount calculator": #If you want a discount calculator, the discountcalculator function will run
    discountcalculator()
  elif whatfunction == "shopping list": #If you want a shopping list, the shoppinglist function will run
    shoppinglist()
  elif whatfunction == "tea": #If you want tea, the tea function will run
    tea()
  
main()
