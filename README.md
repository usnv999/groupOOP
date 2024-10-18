# groupOOP
class Vehicle:
    def __init__(self, speed, color):
        self.speed = speed
        self.color = color

    def move(self):
        raise NotImplementedError("Этот метод должен быть реализован в подклассах")

class Car(Vehicle):
    def move(self):
        return f"Машина {self.color} едет со скоростью {self.speed} км/ч."

class Bike(Vehicle):
    def move(self):
        return f"Велосипед {self.color} крутит педали со скоростью {self.speed} км/ч."

class Boat(Vehicle):
    def move(self):
        return f"Лодка {self.color} плывет со скоростью {self.speed} км/ч."

# Примеры использования
car = Car(100, "красный")
bike = Bike(20, "синий")
boat = Boat(30, "зеленый")

print(car.move())
print(bike.move())
print(boat.move())

