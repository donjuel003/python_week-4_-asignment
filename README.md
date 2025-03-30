# python_week-4_-asignment

def calculate_discount(price, discount_percent):
    """
    Calculates the final price after applying a discount.
    If the discount percentage is 20% or higher, apply the discount;
    otherwise, return the original price.
    """
    if discount_percent >= 20:
        discount_amount = (discount_percent / 100) * price
        return price - discount_amount
    return price

# Prompt user for input
price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))

# Calculate final price
final_price = calculate_discount(price, discount_percent)

# Display result
print(f"Final price after discount: {final_price:.2f}")
