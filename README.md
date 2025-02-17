# Vigenere-Cipher
This image shows a historical cipher table attributed to Blaise Pascal. Its name, “CHIFFRE INDÉCHIFRABLE,” means “Unbreakable Cipher.”

![CipherTable](dictionnairedech00poug_0081.png)

# 🔐 Vigenère Cipher Encoder & Decoder

Tento projekt je jednoduchá webová aplikácia na šifrovanie a dešifrovanie textu pomocou **Vigenèrovej šifry**. Funguje **offline**, všetko sa spracúva priamo v prehliadači.

## 🛠️ Funkcie
- 🔒 **Šifrovanie**: Zadajte text a kľúč, vygeneruje sa zašifrovaný text.
- 🔓 **Dešifrovanie**: Zadajte zašifrovaný text a rovnaký kľúč, dostanete pôvodný text.
- ⚡ **Rýchle a bezpečné**: Nevyžaduje internetové pripojenie, všetko sa vykonáva lokálne v prehliadači.
- 🎨 **Jednoduchý a pekný dizajn**.

## 🚀 Ako používať

1. **Otvorte súbor** `cipher.html` v ľubovoľnom prehliadači.
2. **Zadajte text**, ktorý chcete zašifrovať alebo dešifrovať.
3. **Vyberte kľúč** – rovnaký kľúč musí byť použitý na šifrovanie aj dešifrovanie.
4. Kliknite na **"Šifrovať"** alebo **"Dešifrovať"**.
5. Skopírujte výsledok a použite ho podľa potreby.

## 📜 Čo je Vigenèrova šifra?
Vigenèrova šifra je polyalfabetická substitučná šifra, ktorá používa kľúčové slovo na iteratívne posuny písmen v texte. Je bezpečnejšia ako jednoduchá Caesarova šifra, pretože rovnaké písmeno môže byť zakódované rôznymi spôsobmi.

## 📂 Súbory v repozitári

- `cipher.html` – hlavná stránka s užívateľským rozhraním a šifrovacím skriptom.
- `README.md` – tento popis projektu.

## 📜 Licencia
Tento projekt je open-source a je licencovaný pod **MIT licenciou**. Môžete ho slobodne používať, upravovať a zdieľať. 😊

---


# 🔐 Vigenère Cipher Encoder & Decoder

This project is a simple web application for encrypting and decrypting text using the **Vigenère Cipher**. It works **offline**, everything is processed directly in the browser.

## 🛠️ Features
- 🔒 **Encryption**: Enter text and key, ciphertext is generated.
- 🔓 **Decryption**: Enter ciphertext and the same key, you get the original text.
- ⚡ **Fast and secure**: No internet connection required, everything is done locally in the browser.
- 🎨 **Simple and nice design**.

## 🚀 How to use

1. **Open the file** `cipher.html` in any browser.
2. **Enter the text** you want to encrypt or decrypt.
3. **Select a key** – the same key must be used for encryption and decryption.
4. Click **"Encrypt"** or **"Decrypt"**.
5. Copy the result and use it as needed.

## 📜 What is the Vigenère cipher?
The Vigenère cipher is a polyalphabetic substitution cipher that uses a keyword to iteratively shift letters in a text. It is more secure than a simple Caesar cipher because the same letter can be encoded in different ways.

## 📂 Files in the repository

- `cipher.html` – the main page with the user interface and encryption script.
- `README.md` – this project description.

## 📜 License
This project is open-source and licensed under the **MIT License**. You are free to use, modify, and share it. 😊

---
✨ **If you like this project, give it a ⭐ on GitHub!** ✨

---

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

`./cipher.html`