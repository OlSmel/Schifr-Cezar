# Schifr-Cezar
#Schifr Cezar decryption

key = int(input()) # shift
message = input() # string

for i in message:
    decryption = (ord(i) - key) # ord() convert a character to an int
    if decryption  < 97:
        decryption += 26
    elif decryption > 97:
        decryption -=26
    print(chr(decryption), end='') # convert an integer argument to character
