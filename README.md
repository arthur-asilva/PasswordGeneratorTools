# PasswordGeneratorTools
This package was made to help you with simple daily tasks like generating password suggestions. To use, you need to install the package from pip install password-generator-tools or clone these files.

# Import
Use the below code to import the package into your project after installation:

from PasswordGeneratorTools import PasswordGeneratorTools


# Usage
The package generates full options password from your information length or you can do it with single choices like this:
  - Alphabet characters;
  - Digits;
  - Special characters;
  - Custom the options above;
  - Full generation.

### So, start with call this object like this:
password = PasswordGeneratorTools()

### After, call your single methods like this:

''' this is to define your password length  '''
password_length = 8

''' this is to generate your password length previously defined by you, this method just use alphabet ASCII characters  '''
alphabet_password = password.Alphabet(password_length)

''' this is to generate your password length previously defined by you, this method just use digits (0 to 9)  '''
digit_password = password.Digit(password_length)

''' this is to generate your password length previously defined by you, this method just use special characters like !@#$%^&*()  '''
special_password = password.Special(password_length)

''' this is to generate your password length previously defined by you, this method use all options above  '''
full_character_password = password.CharactersGenerator(password_length)


### You can simplify use a dict with the following keys: 'alphabet', 'digits' or 'special'. Each key will have your attribute length, like this:
params = {
  'alphabet': 3,
  'digits': 3,
  'special' 2
}

### If you need, just use what you want, see below.
params = {
  'alphabet': 4,
  'digits': 4
}

### In this case, your password just will have alphabet and digits characters. I hope help you!
