# team git

🔐 Message Decryption & Threat Detection System
This system consists of three main functions used to decrypt messages, detect dangerous words, and issue a warning based on the threat level.

Functions
1. decrypt_message(encrypted: str) -> str
📌 Description:
Decrypts an encrypted string and returns the original message.

📥 Input:

encrypted (str): The encrypted message string.

📤 Output:

A string (str) representing the decrypted message.

2. analyze_threats(message: str, dangerous_words: list[str]) -> tuple[str, int]
📌 Description:
Checks for the presence of dangerous words in the message. For each dangerous word found, 1 point is added. Returns the message and the total threat points.

📥 Input:

message (str): The decrypted message.

dangerous_words (list[str]): A list of dangerous words to check for.

📤 Output:

A tuple containing:

The original message (str)

The total threat points (int)

3. print_warning(message: str, points: int) -> None
📌 Description:
Prints a warning message based on the total number of threat points.

📥 Input:

message (str): The decrypted message.

points (int): The total number of threat points.

📤 Output:

None (Prints the final message including the warning and point count)

📊 Warning Levels:

1–5 points: WARNING

6–10 points: DANGER!

11–15 points: ULTRA ALERT!

The final printed message includes the decrypted message, the warning level, and the total threat points.
