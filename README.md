# Chat-GPT-Coding
Used to re-create DS-3850 python coding projects using AI (ChatGPT 3.5)

def mad_lib():
    # Prompting user for inputs
    adjective = input("Enter an adjective: ")
    large_objects_plural = input("Enter a plural noun for large objects: ")
    body_part = input("Enter a body part: ")
    restaurant = input("Enter a restaurant name: ")
    first_food = input("Enter a type of food (singular): ")
    second_food = input("Enter another type of food (singular): ")
    large_object_singular = input("Enter a singular noun for a large object: ")

    # Creating the MadLib story with user inputs
    story = f"I’ve had a very {adjective} day. This morning, I dropped a box of {large_objects_plural} on my {body_part}. Then, at lunch, I went to {restaurant} for their delicious {first_food}, but the waiter brought me {second_food}, which I was not hungry for. Finally, on my way home, I was cut off by a van with a large {large_object_singular} strapped to the roof."

    # Displaying the completed MadLib story
    print("\nHere's your MadLib story:\n")
    print(story)

if __name__ == "__main__":
    mad_lib()