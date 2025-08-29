# week-3---discount-calculator

def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = price*(discount_percent/100)
        final_price = price - discount_amount
        return final_price
    else:
        return price

def main():
    price = float(input("ORIGINAL PRICE : "))
    discount_percent = float(input("DISCOUNT APPLIED : "))
    final_Price = calculate_discount(price,discount_percent)
    if final_Price < price:
      print(f"The final price after applying {discount_percent} % is {final_Price}")
    else:
      print(F"No discount was applied and original price is {price}")
main()
