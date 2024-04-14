def calculate_simple_interest(principal, rate, time):
    """
    Calculate simple interest.

    Args:
    principal (float): The principal amount.
    rate (float): The interest rate (as a percentage).
    time (float): The time period (in years).

    Returns:
    float: The simple interest.
    """
    interest = (principal * rate * time) / 100
    return interest

def main():
    principal = float(input("Enter the principal amount: "))
    rate = float(input("Enter the interest rate (in percentage): "))
    time = float(input("Enter the time period (in years): "))

    interest = calculate_simple_interest(principal, rate, time)
    total_amount = principal + interest

    print(f"\nSimple Interest: {interest}")
    print(f"Total Amount: {total_amount}")

if __name__ == "__main__":
    main()
