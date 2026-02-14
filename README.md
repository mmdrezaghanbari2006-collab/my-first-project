# my-first-project
# راه اول نشان دادن اعداد اول

def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True


print(is_prime(1000))  # True


# راه دوم نشان دادن اعداد اول

n = 1000
flag = 1
i = 2
while (i < n):

    if n % i == 0:

        flag = 0

    i = i + 1
if flag == 1:

    print("prime")

if flag == 0:

    print("not prime")


# راه سوم نشان دادن اعداد اول


num = 1000

# فرض اولیه: عدد اول است
flag = 1

i = 2
while i < num:
    if num % i == 0:
        flag = 0  # عدد بخش‌پذیر شد => اول نیست
        break
    i += 1

if flag == 1 and num > 1:
    print("prime_number")
else:

    print("not_prime_number")
