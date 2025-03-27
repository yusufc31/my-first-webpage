# my-first-webpage
This site is about gay test if you are not gay u will pass it and will be succesful
def gay_test():
    print("Welcome to the Gay Test!")
    print("Please answer the following questions with 'yes' or 'no'.")

    questions = [
        "Do you enjoy watching romantic movies?",
        "Do you have a crush on a celebrity?",
        "Do you like fashion and shopping?",
        "Have you ever been to a pride event?",
        "Do you enjoy dancing at parties?"
    ]

    gay_score = 0

    for question in questions:
        answer = input(question + " ").strip().lower()
        if answer == 'yes':
            gay_score += 1
        elif answer != 'no':
            print("Please respond with 'yes' or 'no'.")

    print("\nYour results:")
    if gay_score > 2:
        print("Unlucky for you! You seem to have some gay tendencies.")
    else:
        print("Congratulations! You appear to be not gay.")

if __name__ == "__main__":
    gay_test()
