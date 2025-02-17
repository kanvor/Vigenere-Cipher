# Vigenere-Cipher
This image shows a historical cipher table attributed to Blaise Pascal. Its name, “CHIFFRE INDÉCHIFRABLE,” means “Unbreakable Cipher.”

![CipherTable](dictionnairedech00poug_0081.png)

What does the table contain?

• A large table with double letters (probably a Vigenère or Playfair cipher).

• The French text below the table explains the principle of encryption:

• You use a secret word (in the example, “Paris”).

• The encryption works by shifting each letter according to the secret word.

• The result is unintelligible words that can only be deciphered with the key.

Translation of the French text below the table:

The use of this cipher is based on an agreed-upon word that can be changed letter by letter on each line.

Example:

Let’s assume the agreed-upon word is Paris.

• Je veux écrire… (I want to write…) → Vous serez demain au rendez-vous. (We will meet tomorrow.)
• Je mets… (I give…) → Pari s pari sparis pa rispar ispa.
• Voici ce que j’écris… (This is what I write…) → Umyq alini ploraf pé aefmxt oeuh.
• Celui qui recogniz la lettre met… (The recipient decrypts…) → Pari spari sparis pa rispar ispa.

And finally he says:

If UP is said, it means U. If MA is said, it means O.

What does it mean?

• It is probably a historical form of the Vigenère cipher.
• The secret word Paris is used to shift the letters in the message.
• The result is a seemingly random text that is only readable with the key.

---

This looks like a historical polyalphabetic cipher, probably the Vigenère cipher, which is considered one of the most important in the history of cryptography. It is called the “Chiffre Indéchiffrable” (Unbreakable Cipher) because at the time of its creation it was considered practically unbreakable. Today we know that it is not completely secure, but it is still very interesting!

How does this cipher work?

The Vigenère cipher is an extension of the Caesar cipher, but with the letters shifting according to the keyword.
1. You choose a secret word (e.g. “PARIS”).
2. You type the original text (e.g. “HELLO”).
3. The key word is repeated to be the same length as the message:

Message: H E L L O
Key: P A R I S

4. Each letter is shifted by the value of the key letter:
• H (P shift) → W
• E (A shift) → E
• L (R shift) → C
• L (I shift) → T
• O (S shift) → G
The resulting encrypted message is “WECTG”.
5. To decrypt, simply subtract the shift in the opposite direction.

The table we see in the picture

It looks like a cipher table (also called a Vigenère table or shift table). It works like this:
• The rows and columns contain the alphabet.
• Each letter is replaced by the letter at the intersection of the row (original letter) and the column (key word).
• This allows for more complicated encryption, where the offsets change for each character.

Why was it considered unbreakable?
• Unlike the Caesar cipher, where the offset is always the same, the Vigenère cipher changes the offset for each letter.
• Statistical analyses of letter frequencies (which work for simple ciphers) are almost useless here.
• It took hundreds of years to find an effective way to break it.

Is it secure today?
• Not entirely - it was broken in the 19th century by the Kasiski test and the Friedman coincidence index.
• Much more secure ciphers than AES are used today.
• Nevertheless, the Vigenère cipher is great for understanding the principles of cryptography.

Want to try it? :)

./cipher.html