# rune-keeper
A private vault for storing and managing sensitive keys, secrets, and credentials. Secure, encrypted, and guarded like ancient runes. 🏰✨

## Working
The migaku takes the env files from rune-keeper. The runes (env files) needed for the projects should be saved in rune-keeper inorder for migaku to use it. The runes should be saved following these 3 conditions
 - The runes should be saved in the folder with the name same as the repo name of the project it belongs to
 - The runes should be saved as enc file using the encryption command given below
 - The name of the enc file will be same as the rune with an added extension of .enc
    
    `openssl enc -aes-256-cbc -e -pbkdf2 -salt -in "$SOURCE_FILE" -out "$ENCRYPTED_FILE" -pass stdin`