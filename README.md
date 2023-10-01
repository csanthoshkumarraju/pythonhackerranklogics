# def print_full_name(first,last):
#     return " Hello " + first + last+  " You just delved into python. "
# first = input()
# last = input()
# a = print_full_name(first,last)
# print(a)
# def split_and_join(line):
#     # write your code here
#     return jn
# st = input()
# sp = st.split(" ")
# jn = "-".join(sp)
# b = split_and_join(st)
# print(b)
# s = 'aGFABSVjhgjghf'
# sw = s.swapcase()
# print(sw)
# s = 'santhosh2'
# print(s.isalpha())
# s = 'ABCDCDC'
# ss = 'CDC'
# l = len(s)
# if ss in s:
#     print(s.count(ss,0,l))
# else:
#     print('false')
# i = 5
# for i in range(1,i+1):
#      print(i)
# n = input('enter number countries:--')
# print(n, ' countries')
# names = [str(names) for names in input("enter "+ ' '+ str(n) +" country names:-").split()]
# print(names)
# dcountries = set(names)
# print(len(dcountries))

# s = 'santgosh'
# o = s.replace(s[4],'h')
# print(o)
# n = int(input())
# lst =[]
# for i in range(0,n):
#     ele = int(input())
#     lst.append(ele)
# # print(lst)
# he = max(lst)
# rh = lst.remove(he)
# # print(lst)
# print(max(lst))

# s = {1,2,3,4,5,6,7,7,6,3}
# su = sum(s)
# l = len(s)
# print(su/l)
# s = set(map(int, input().split()))
# print(s)
# # pop remove discard
# p = s.pop()
# print(p)
# r = s.remove(s[3])
# print(r)
# d= s.discard(s[5])
# print(d)
# en = set(map(int, input().split()))
# fr = set(map(int, input().split()))
# u = en.union(fr)
# print(len(u))

# n = int(input('enter number of students'))
# marks =[]
# for i in range(1,n):
#     ele = int(input('enter marks of '+ str(i) +' '+ 'student'))
#     marks.append(ele)
# print('studen marks are :--\n',marks)
# hm = max(marks)
# print('highest marks',hm)
# sh = marks.remove(hm)
# print('removed highest marks',sh)
# print('without first highest marks',marks)
# print('second highest marks',max(marks))
# s1 = {1,2,3,3,4,5,6}
# s2 = {3,4,5,10,1,11,12,13}
# print(s1 - s2)
# es = set(map(int, input().split()))
# fs = set(map(int, input().split()))
# print(es)
# print(fs)
# print(es - fs)
# print(len(es - fs))
# en = int(input)
# es = set(map(int, input().split()))
# fn = int(input)
# fs = set(map(int, input().split()))
# diff = es - fs
# print(len(diff))

# n = int(input('enter the count of phone numbers:--'))
# print('your count of  phone numbers:--',n)
# cp =input('Please enter 10 digits with numbers only.').split()
# print('your numbers are:--',cp)
# for i in cp:
#    if i.isalnum() and len(i) == 10 and (i[0] ==7 or i[0] ==8 or i[0] ==9):
#       print('yes')
#    else:
#       print('your number is not a number or digits are less than 10 or Not starting with 7,8,9')
#       print('please try again')
# ----------------
# l = ['7893062057','7019487853']
# for fd in l:
#    print(fd[0])
# -----------
# l = [7893062057,7019487853]
# for fd in l:
#    sfd = str(fd)
#    print(sfd[0])
#    fc = sfd[0]
# print(fc)
# if fc in [7,8,9]:
#    print('True')
# else:
#    print('False')







# import math
# import os
# import random
# import re
# import sys
#
#
# class Item:
#     # Implement the Item here
#     name = ''
#     price = 0
#
#     def __init__(self, f, p):
#         self.f = f
#         self.p = p
#
#     pass
#
#
# class ShoppingCart:
#     # Implement the ShoppingCart here
#     cart_names = []
#     cart_prices = []
#     tot = 0
#
#     def __init__(self):
#         super().__init__()
#
#     def add(self, item):
#         self.cart_names.append(item.name)
#         self.cart_prices.append(item.price)
#
#     def total(self):
#         self.tot = sum(self.cart_prices)
#         return self.tot
#
#     def __len__(self):
#         return len(self.cart_names)
#
#     pass
# g = Item(7,8)
# print(g)
class Item:
    def __init__(self,name: str,price: int):
        self.name = name
        self.price = price
class ShoppingCart:
    def __init__(self, item: Item):
        self.items = []
    def add(self, item: Item):
        self.items.append(item)
    def total(self) -> int:
        return sum(item.price for item in self.items)
    def __len__(self):
        return len(self.items)
