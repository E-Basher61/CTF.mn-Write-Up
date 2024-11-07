# CTF.mn WriteUp

## First Blood

📄**Category: Cryptography**  
🏆**Event/Contest: Харуул Занги U18 - 2022**  
✍️**Author: Flame**  
📰**Info: Legends says that flame managed to draw first blood in 4 seconds.**  
📗**Given: `86T"J3.#6l0lh>W?Xdh*0JI$EARmJTAN2M+1OT`**  
🔗**Link: [First Blood](https://ctf.mn/challenge/3)**

![{First Blood}](https://github.com/user-attachments/assets/3f3da02f-fa88-43c0-a078-88e66fee503e)

# Solving Guide

1. We can see that the given data is a string of characters that could be:
	- An Encrypted Message or Hash
 	- Random Key or Password
  	- Hexadecimal-Encoded or Base64-Like Data
   	- Obfuscated Data
   	  
   	![{String}](https://github.com/user-attachments/assets/b1f6e97a-633b-4db0-b5da-7033e8b8cbcc)
  
2. We can use a decoding website or tool to achieve our goal, acquiring the flag
	- **[CyberChef](https://gchq.github.io/CyberChef/)**: Insert the string into the "Input" and press "Magic" on the left side, to find out what type of encoding was used.
 	- **[dCode](https://www.dcode.fr/en)**: The same process as the previous one. After decoding the string, we will result in acquiring the flag.

	![{Input}](https://github.com/user-attachments/assets/b281f861-0bba-46db-b30c-c824f89449bc)

	![{Magic}](https://github.com/user-attachments/assets/3631b824-926b-4674-a118-6e3bbf8ca133)

	![{Flag}](https://github.com/user-attachments/assets/d453f58a-da5b-4cca-8e8c-b1efb98cc6f9)

3. Now we can see that the "Base85" encoding method was used. In addition, we have found our flag.
	- Flag: `HZU18{f11rst_bl000d_ed09e8483}`

# Good Luck! Hack Away!
