# Homework_6.3


def multiply_digits_until_single_digit(number):
    while number > 9:
        product = 1
        for digit in str(number):
            product *= int(digit)
        number = product
    return number

print(multiply_digits_until_single_digit(999))   # 2
print(multiply_digits_until_single_digit(1000))  # 0
print(multiply_digits_until_single_digit(423))   # 8
print(multiply_digits_until_single_digit(33))    # 9
print(multiply_digits_until_single_digit(25))    # 0
print(multiply_digits_until_single_digit(1))     # 1
