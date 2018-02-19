# exercise-6-string-lists
# Still learning python
# Get an input
string = input("Give me a word or phrase:")

def reverse(test):
  """test the string to see if it's a palindrome.  Only looks at letters & numbers."""
  test_string = test.lower()
  test_char = "0123456789abcdefghijklmnopqrstuvwxyz"
  fwd = ""
  for char in test_string:
    if char in test_char:
      fwd = fwd + char
  rev = fwd[::-1]
  if fwd == rev:
    print("You gave me a palindrome!!")
  else:
    print("That is not a palindrome.")
    
reverse(string)
