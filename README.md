words = ["void", "echoes", "fragment", "shattered", "whispers", "oblivion", "forgotten", "dusk", "rift", "hollow"]
symbols = ["@", "#", "$", "%", "&", "*", "!", "?"]

def generate_message():
    message = " ".join(random.choice(words) for _ in range(5))
    scrambled = "".join(random.choice(symbols) if random.random() > 0.7 else char for char in message)
    return scrambled.capitalize()

print(generate_message())
