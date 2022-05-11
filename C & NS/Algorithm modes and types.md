- ### Steam cipher -
	This Encrypt the message one plain bit at a time. bit by bit encryption.
- ### Block cipher-
	In this we encrypt one block of byte at a time.
	
	
#### Algorithm modes
- **Electronic code book (ECB):** BLOCK CIPHER
	- Steps:
		- First the plain text is devided into **64 bit blocks **.
		- them it encrypt the blocks using its encryption technique.
		### Note: Single key is used to encrypt all the blocks
		
- **cipher block chaining mode (CBC)**: BLOCK CIPHER:
	- Uses initialization vector and feedback mechanism
	- First the plain text is devided into **64 bit blocks **.
	- now suing IV we get one text, now use encryption on this algorithm on this text to get encrypted data.
	- this encryptes data will work as a IV of next block.
	
- **cipher feed block mode (CFB)**: BLOCK CIPHER but acty as stream cipher
	- Updated version of CBC.
	- Get IV(given)
	- Encrypt the IV using encryption mechanism
	- choose first j bit of encrypted IV and plain text and create a final text using them.
	- now use left shipf on IV upto j bit.
	- now replace the open part in Iv bym the encrypted text recieve before.
- **output feedback (OFB)** : BLOCK CIPHER but act as stream cipher
	- Same as bnefor, only one stepo is changed.
	- instead of passing encrypted text to the next iv, we pass encoded iv to the next step

- Counter Mode (CTR):
 here we use counter.
 - encrypt counter.
 - now use encrypted counter and plain text to get encrypted text.
 - in next blocks counter value will be encreased by 1.