# morse-code-translator
# Defining the Morse code alphabet
morse_code = {
    '.-': 'A', '-...': 'B', '-.-.': 'C', '-..': 'D', '.': 'E',
    '..-.': 'F', '--.': 'G', '....': 'H', '..': 'I', '.---': 'J',
    '-.-': 'K', '.-..': 'L', '--': 'M', '-.': 'N', '---': 'O',
    '.--.': 'P', '--.-': 'Q', '.-.': 'R', '...': 'S', '-': 'T',
    '..-': 'U', '...-': 'V', '.--': 'W', '-..-': 'X', '-.--': 'Y',
    '--..': 'Z', '-----': '0', '.----': '1', '..---': '2', '...--': '3',
    '....-': '4', '.....': '5', '-....': '6', '--...': '7', '---..': '8',
    '----.': '9', '--..--': ',', '.-.-.-': '.', '..--..': '?', '-..-.': '/',
    '-....-': '-', '-.--.': '(', '-.--.-': ')'
             }

# Getting the Morse code input from user
def get_input1():
    print("Enter the Morse code (using dots for '.' and dashes for '-'), separate characters with space:")
    input1 = input().strip().split()
    return input1

# Translating the Morse code to English
def morse_to_english(input1):
    output = []
    for morse_char in input1:
        eng_char = morse_code.get(morse_char.upper()
    # changing the input to uppercase 
        if eng_char:
            output.append(eng_char)
        else:
            output.append('[UNKNOWN]')
    return ''.join(output)

# Main program
if __name__ == "__main__":
    input1 = get_input1()
    translated_text = morse_to_english(morse_input)
    print("Translated to English:", translated_text)
