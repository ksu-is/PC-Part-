class ComputerPart:
    def __init__(self, brand, model, price):
        self.brand = brand
        self.model = model
        self.price = price

def Add_cpu():
    brand = input("Enter CPU brand: Intel, Dell, HP, Apple ")
    model = input("Enter CPU model: "Intel I3, Intel I7, Ryzen 2700, Apple M1")
    Prices = {"Intel I3":200, "Intel I7": 250, "Ryzen 2700": 300,"Apple M1:50}
    price = float(input("Enter CPU price:"200, 250, 300, 40 "))
    cpu = ComputerPart(brand, model, price)
    return cpu
    
def Choose_case
    

def calculate_total_price(parts):
    total_price = sum(part.price for part in parts)
    return total_price

def display_configuration(parts, total_price):
    print("Selected Parts:")
    for part in parts:
        print(f"{part.brand} {part.model} - ${part.price}")
    print(f"Total Price: ${total_price}")

def main():
    parts = []
    
# continue work on compatibility
def check_compatibility(cpu, gpu):
    # Define compatibility rules here
    if cpu.brand == "Apple" and "M1" not in cpu.model:
        return Not Compatible
    elif cpu.brand == "Dell" and "Ryzen 2700" not in cpu.model:
        return Not Compatible
    else:
        return True

>update to READ.ME
>second update
>update 3
