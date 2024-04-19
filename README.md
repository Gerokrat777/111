class Car:

    def __init__(self, powers=150):
        self.price = 1000000
        self.powers = powers

    def __str__(self):
        return f'цена на данный автомобиль =  {self.price}\n'\
        f'мощность двигателя =  {self.powers}'

    def horse_powers(self):

        return self.powers



class Nissan(Car):

    def __init__(self, price=750000):
        super().__init__(price)
        self.price = price

    def horse_powers(self):
        self.powers = 550



class Kia(Car):

    def __init__(self):
        super().__init__()
        self.price = 800000

    def horse_powers(self):
        self.powers = 300




obj = Car()
obj.horse_powers()
print(obj)

obj_ = Nissan()
obj_.horse_powers()
print(obj_)

obj__= Kia()
obj__.horse_powers()
print(obj__)
