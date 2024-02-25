<<<<<<< HEAD
# Chat-GPT-Coding
Used to re-create DS-3850 python coding projects using AI (ChatGPT 3.5)

def run_quiz():
    # Define the quiz questions and answers as a dictionary
    quiz_questions = {
        "What is the capital of France?": "Paris",
        "True or False: The Earth is flat.": "False",
        "What is the largest mammal?": ["A. Elephant", "B. Blue Whale", "C. Giraffe", "D. Lion"],
        "What is the chemical symbol for water?": "H2O",
        "Fill in the blank: The mitochondria is the _______ of the cell.": "powerhouse"
    }

    # Initialize counters for correct and incorrect answers
    correct_count = 0
    total_questions = len(quiz_questions)

    # Iterate through the questions and ask them one by one
    for question, answer in quiz_questions.items():
        print(question)
        
        # If it's a multiple choice question
        if isinstance(answer, list):
            for choice in answer:
                print(choice)
            user_answer = input("Enter the letter of your choice: ").upper()

            # Check if the user's choice is valid
            while user_answer not in ['A', 'B', 'C', 'D']:
                print("Invalid choice. Please enter A, B, C, or D.")
                user_answer = input("Enter the letter of your choice: ").upper()

            user_answer_idx = ord(user_answer) - ord('A')  # Convert letter to index
            user_answer = answer[user_answer_idx][3:]  # Get the choice text without the letter
        else:
            user_answer = input("Your answer: ")

        # Check if the answer is correct
        if isinstance(answer, list):
            correct = user_answer.lower() == answer[1][3:].lower()  # Assuming the second choice is the correct one
        else:
            correct = user_answer.lower() == answer.lower()
        
        # Provide feedback on the answer
        if correct:
            print("Correct!\n")
            correct_count += 1
        else:
            print(f"Incorrect. The correct answer is: {answer}\n")

    # Display final results
    print("Quiz completed! Thanks for playing.")
    print(f"You got {correct_count} out of {total_questions} questions correct.")

if __name__ == "__main__":
    run_quiz()
=======

>>>>>>> d9b73b2a510b58875bb5321170c7eaa1f1d6cd56
