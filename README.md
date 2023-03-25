# -ki-say-l-basit-hesap-makinesi-Python-
Python ile yazılmış, iki sayı ile çalışan bir hesap makinesi

Source code:

import sys

sys.set_int_max_str_digits(999999999)

num1 = int(input("İlk sayıyı giriniz:"))
num2 = int(input("İkinci sayıyı giriniz:"))
prcs = str(input("""Yapacağınız işlemi seçiniz;
Toplama  (+)
Çıkarma  (-)
Çarpma   (*)
Bölme    (/)
Üst Alma (**)
:"""))

while True:
    if prcs == "+":
        print(f"{num1} + {num2} = {num1+num2}")
        break
    elif prcs == "-":
        print(f"{num1} - {num2} = {num1-num2}")
        break
    elif prcs == "*":
        print(f"{num1} * {num2} = {num1*num2}")
        break
    elif prcs == "/":
        print(f"{num1} / {num2} = {num1/num2}")
        break
    elif prcs == "**":
        print(f"{num1} ** {num2} = {num1**num2}")
        break
    else:
        print("HATALI İŞLEM!!!")
    prcs = str(input("""Yapacağınız işlemi seçiniz;
Toplama  (+)
Çıkarma  (-)
Çarpma   (*)
Bölme    (/)
Üst Alma (**)
:"""))
