return_rate = float(input('What is your minimum rate of return? : '))
current_divident = float(input("what is the current year dividend? : "))
growth_rate = float(input("What is the growth rate? : "))
future_dividend = current_divident * (1 + growth_rate)
intrinsic_value_DDM = (future_dividend)/(return_rate-growth_rate)
current_market_price = int(input('What if the current market price of the stock? : '))
if (intrinsic_value_DDM == current_market_price):
    print("Stock is fairly valued, hold your current position")

elif(intrinsic_value_DDM > current_market_price):
    print("Stock is undervalued, you can purchase the stock at the current price")
else:
     print("Stock is overvalued, not advisable to purchase the stock at the current price")
input()



     
     
