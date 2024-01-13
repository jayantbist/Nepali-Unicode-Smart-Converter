# Sample character mapping (you may need to expand this)
nepali_mapping = {
    'a': 'अ',
    'b': 'ब',
    # Add more mappings as needed
}

def convert_to_unicode(input_text):
    unicode_text = ''
    for char in input_text:
        unicode_text += nepali_mapping.get(char, char)
    return unicode_text

# Example usage
nepali_input = input("Enter Nepali text: ")
unicode_output = convert_to_unicode(nepali_input)
print("Unicode Output:", unicode_output)
