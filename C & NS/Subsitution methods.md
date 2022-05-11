- Ceaser cipher: the shift cipher, the shipt is defined in the 26 alphabets.
It is a type of substitution _cipher_ in which each letter in the plaintext is replaced by a letter some fixed number of positions down the alphabet. position is always 3 down

- Modified version of ceaser cipher: the major difference is the shift is not nessasarily 3, it can be changed.

- Monoalphabetic cipher: A monoalphabetic cipher is any cipher in which the letters of the plain text are mapped to cipher text letters based on a single alphabetic key. here we can specify which letter will be converted to which. ex- A will convert to c and b will convert to X.

- polyalphabetic cipher: A polyalphabetic cipher is any cipher based on substitution, using multiple substitution alphabets. here we can specify a block of letter(word).
ex- HI will convert to TO.

- Homophoric substitution: The Homophonic Substitution cipher is a substitution cipher in which single plaintext letters can be replaced by any of several different ciphertext letters.
ex- A can be converted to {X,Y,H,G} any of these chacters.

- polyalphabetic substitution cipher(Vigenere cipher): A polyalphabetic cipher is any cipher based on substitution, using multiple substitution alphabets.
	- here we uses key and a table to encrypt and decrypt data.

![[Pasted image 20220510225930.png]]

- Playfair substitution method: In playfair cipher unlike traditional cipher we encrypt a pair of alphabets(digraphs) instead of a single alphabet.
	- Creation of population matrix (5*5 size)
	- encryption method

Steps:
- create a table of 5 * 5.
- fill chacter in block. chacter must not repeate.
- if data is not filled completely, add remaining chacters from 26 chacters of english (I and J willl be considered as a single column.) 

Encryption process: 
- devide your input text in group of two characters.
- if two alfabets are same or last remaining set has only one alfabet, replace one alfabet by X or add x in the end.

Rules to check new elements from matrix
- if both alphabets are in same row then replace them with element right next to them.
- if boath alphaboths are in same column then replace them the element down below them.
- if they are not in same column or row, they will be replaced by diagonal character


- Hill cipher:  the Hill cipher is a polygraphic substitution cipher based on linear algebra.
	- Steps of encryption:
		- define numeric values to each element
		- convert your text into numbers.
		- create a mtrix using these values.
		- multiply this with key martrix.
		- devide the each element value by 26.
		- now convert the remainder into text,this is the encrypted value.

For decryption:
- do same as above
- except our key matrix will be inverse of original key matrix.