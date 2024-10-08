def chatbot_response(user_input):
    user_input = user_input.lower()

    if "hello" in user_input or "hi" in user_input:
        return "Hello! How can I help you today?"
    elif "how are you" in user_input:
        return "I'm just a program, but I'm functioning as expected! How about you?"
    elif "your name" in user_input:
        return "I'm Chatbot, your friendly assistant!"
    elif "bye" in user_input or "exit" in user_input:
        return "Goodbye! Have a nice day!"
    else:
        return "I'm not sure I understand. Can you please rephrase?"

def main():
    print("Welcome to Chatbot! Type 'bye' or 'exit' to end the chat.")
    while True:
        user_input = input("You: ")
        response = chatbot_response(user_input)
        print("Chatbot:", response)

        if "bye" in user_input or "exit" in user_input:
            break


if __name__ == "__main__":
    main()
