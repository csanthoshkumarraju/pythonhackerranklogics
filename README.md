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
