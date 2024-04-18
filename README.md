def is_prime(number):
    if number <= 1:
        return False
    for i in range(2, int(number**0.5) + 1):
        if number % i == 0:
            return False
    return True

if __name__ == "__main__":
    num = int(input("Digite um número: "))
    if is_prime(num):
        print(f"{num} é primo!")
    else:
        print(f"{num} não é primo.")
