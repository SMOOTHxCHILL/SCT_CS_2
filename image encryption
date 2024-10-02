def endec(path, key) :
    fin = open(path, 'rb') #images are read through rb as the contents are read as a stream of bytes
    image = fin.read()
    fin.close()
    image = bytearray(image) #converts stream of bytes to a mutable stream
    
    for index, values in enumerate(image) : #enumerate seperates each byte from the next and assigns an index to it which makes the XOR operation possible
        image[index] = values ^ key #^ performs XOR operation; ** is expotentiation
        
    fin = open(path, 'wb')
    fin.write(image)
    fin.close()

print("What\'s good")
while True :
    inp = int(input("Select 1 for encryption, 2 for decryption and 3 to exit\n"))
    if inp == 1 :
        path = input("Enter the path of the image to be encrypted(without quotation marks):\n")
        key = int(input("Enter the key for encryption:\n"))
        print("Path given is ", path)
        print("Key used for encryption is ", key)
        endec(path, key)
        print("Encrypted successfully\n")
        exit
    elif inp == 2 :
        path = input("Enter the path of the image to be decrypted(without quotation marks):\n")
        key = int(input("Enter the key for decryption:\n"))
        print("Path given is ", path)
        print("Key used for decryption is ", key)
        endec(path, key)
        print("Decrypted successfully\n")
        exit
    elif inp == 3 :
        print("Byee<3")
        break
    else :
        print("Incorrect input given. Try again or enter 3 to exit\n")
