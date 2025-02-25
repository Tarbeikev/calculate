# calculat
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = price * (discount_percent / 100)
        final_price = price - discount_amount
        return final_price
    else:
        return price

# Prompt the user to enter the original price and discount percentage
original_price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))

# Calculate the final price
final_price = calculate_discount(original_price, discount_percent)

# Print the final price or the original price if no discount was applied
if discount_percent >= 20:
    print(f"The final price after applying the discount is: {final_price}")
else:
    print(f"No discount applied. The original price is: {original_price}")
e
