# animal-quiz.
#animal Quiz is a simple string,input,print code
def list_o_matic(animal, animal_list):
    if animal == "":
        removed_item = animal_list.pop()
        return f"{removed_item} popped from list"
    elif animal in animal_list:
        animal_list.remove(animal)
        return f"1 instance of {animal} removed from list"

animal_list = ['cat', 'goat', 'cat' , 'dog' , 'elephant']

print("Welcome, [Ryan Cloninger]. Look at all the animals", animal_list)
while animal_list:
    animal_input = input("enter the name of an animal (type 'quit' to exit): ").lower()
    if animal_input == 'quit':
        break
    else:
        print(list_o_matic(animal_input, animal_list))
print("Goodbye!")
