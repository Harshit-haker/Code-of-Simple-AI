# Code-of-Simple-AI
AI program that uses rule-based logic to answer questions about a fictional animal
# Define the rules for the AI
rules = {
    "is the animal a mammal?": "yes",
    "does the animal have wings?": "no",
    "does the animal live in the ocean?": "no",
    "does the animal have four legs?": "yes"
}

# Define a function to ask the AI a question
def ask(question):
    # Check if the question has a known answer
    if question in rules:
        # Return the known answer
        return rules[question]
    else:
        # Return a default answer
        return "I'm not sure."

# Test the AI by asking it some questions
print(ask("is the animal a mammal?"))  # Output: "yes"
print(ask("does the animal have wings?"))  # Output: "no"
print(ask("does the animal live in the ocean?"))  # Output: "no"
print(ask("does the animal have four legs?"))  # Output: "yes"
print(ask("does the animal have fur?"))  # Output: "I'm not sure."
