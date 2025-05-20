import time

# Welcome message
print("Welcome to my Six60 quiz!")
time.sleep(1)

# Chances
chances = 1
print("You will have", chances, "chance to answer each question.\n")
time.sleep(2)

# Score
score = 0

# Quiz Questions (store both letter and full answer)
quiz_questions = [
    {
        "question": "1) What year was Six60 formed?",
        "options": {
            "a": "2008",
            "b": "2006",
            "c": "2010",
            "d": "2012"
        },
        "answer_letter": "a",
        "answer_text": "2008"
    },
    {
        "question": "2) Which NZ city did Six60 originate from?",
        "options": {
            "a": "Auckland",
            "b": "Wellington",
            "c": "Dunedin",
            "d": "Christchurch"
        },
        "answer_letter": "c",
        "answer_text": "Dunedin"
    },
    {
        "question": "3) How many members are there?",
        "options": {
            "a": "4",
            "b": "6",
            "c": "3",
            "d": "7"
        },
        "answer_letter": "b",
        "answer_text": "6"
    },
    {
        "question": "4) What was Six60's 2020 documentary called?",
        "options": {
            "a": "Don't Forget Your Roots",
            "b": "Rise Up",
            "c": "Forever",
            "d": "Till the Lights Go Out"
        },
        "answer_letter": "d",
        "answer_text": "Till the Lights Go Out"
    },
    {
        "question": "5) Which song did Six60 re-record in Te Reo Maori for Waiata/Anthems?",
        "options": {
            "a": "Sundown",
            "b": "Don't Forget Your Roots",
            "c": "Purple",
            "d": "Mothers Eyes"
        },
        "answer_letter": "b",
        "answer_text": "Don't Forget Your Roots"
    }
]

# Loop through each question
for q in quiz_questions:
    print(q["question"])
    for key, value in q["options"].items():
        print(f"({key}) {value}")
    print()

    for i in range(chances):
        answer = input("Answer: ").strip().lower()
        correct_letter = q["answer_letter"]
        correct_text = q["answer_text"].lower()

        # Check if user input matches letter or full text
        if answer == correct_letter or answer == correct_text:
            print("Correct!\n")
            score += 1
            break
        else:
            print("Incorrect!\n")
            time.sleep(0.5)
            print("The correct answer is", f"({correct_letter}) {q['answer_text']}", "\n")
    
    time.sleep(2)

# Final Score Output
if score >= 2:
    print("Well done! Your score is", score)
else:
    print("Better luck next time! Your score was", score)

# Goodbye
print("Thank you for playing!")
