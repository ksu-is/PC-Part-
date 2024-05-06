class ComputerPart:
    def __init__(self, brand, model, price):
        self.brand = brand
        self.model = model
        self.price = price

def Add_cpu():
     brand = input("Enter CPU brand (Intel, Dell, Apple, HP): ")
    model = input("Enter CPU model (Intel I3, Intel I7, Ryzen 2700, Apple M1): ")
    prices = {"Intel I3": 200, "Intel I7": 250, "Ryzen 2700": 300, "Apple M1": 40}
    price = prices.get(model, 0) 
    cpu = ComputerPart(brand, model, price)
    return cpu
    
def add_case(cpu):
    if cpu.brand == "Apple":
        case_model = "Apple Case"
        case_price = 250
    else:
        case_model = input("Enter case model (Small, Medium, Large): ")
        case_prices = {"Small": 50, "Medium": 75, "Large": 100}
        case_price = case_prices.get(case_model, 0)  
    case = ComputerPart("Apple", case_model, case_price)
    return case

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
    cpu = add_cpu()
    parts.append(cpu)
    case = add_case(cpu)
    parts.append(case)
    total_price = calculate_total_price(parts)
    display_configuration(parts, total_price)
    
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
>update
