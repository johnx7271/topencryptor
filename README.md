# Top Encryptor

This encryption tool is for encrypting **top secret**, i.e. secrets of strategic importance to a country (no objection if you use a cannon to shoot mosquitoes). It is the most powerful and strongest encryption tool in the world. Its strength is 10 to 154th power (10^154) times that of the mainstream encryption: Aes256.

**So, why should we use such a strong and powerful encryption tool?**

The short answer is, why not? It does not cost much as compared with commonly-in-use encryption tools, but it adds much peace of mind to you, assuring you with a full 100% confidence that your secrets encrypted by this can never be cracked by anyone in the world, for now and long after the post quantum computing times, so you can sleep well and never be bothered again by the possibility of losing secrets due to encryption tools weakness or loopholes, known now or to be discovered in the future.

If you have ever been dealing with secrets of this type, I guess you may have worried about the security of common encryption tools. 

Because the current mainstream encryption algorithm is selected by NIST of USA, and this organization has stains in its history. If the algorithm it selects contains loopholes or vulnerabilities that's  known only to itself, then everything encrypted by this algorithm will be visible to the government of USA. Completely trusting the algorithm selected by USA is like entrusting a cat with the custody of fish. 

Also, today's mass storage is getting cheaper, so adversaries may collect your data that you think is safely encrypted, as cryptograph research goes deeper and deeper, someone may discover a way to break the algorithm out of the blue in the future, like this has happened to the DES algorithm, MD6 etc. 

Even if you use non-mainstream encryption algorithms (for example, China, Russia both have its own set of encryption algorithms), it is also worrisome. Because it is non mainstream, there are fewer people to study it. Therefore, the probability of its weaknesses and vulnerabilities being discovered is lower. However, the fact that it is not found now by the public does not mean that the algorithm can be trusted to withstand the cracking and studying of powerful countries using its full national resource (Some choose to keep the algorithms private to themselves, but this also does not add much strength. One of the principles of modern cryptography, Kerckhoffs' principle says: Don't rely on secrecy of algorithms to ensure the security of the system).

On the other hand, the protection of top secret must be foolproof and absolutely safe. The loss of confidentiality of information is often fatal, while the confidentiality of top secret is vital to the fortune of a nation. Although the consequences of information leakage were not immediately visible, they were truly disastrous. For example, the Enigma cipher machine of Germany was cracked, which led to the sinking of numerous German submarines and the soldiers' burial at the ocean floor. The cipher system of Japan was cracked during world war II, which led to the interception and shooting down of the plane carrying Yamamoto 56, the top commander of the Japanese army.

Encryption algorithm is the key to confidentiality. If the encryption algorithm is cracked, its harm is huge, comprehensive and durable, because the party who cracked will try to disguise like it has not cracked. After the Allies had cracked the Enigma cipher machine, they used this strategy. Therefore, countless confidential German information was leaked like water, while Germany was unaware of this fact.

This encryption software is just to help you completely eliminate the above worrying. Even if the encrypted ciphertext is sent to the CIA, the most powerful and famous organization in the field of cracking secret in the world, you can still sleep sound and easy. This software is unique, reliable and absolutely secure.

## Application scenario:
1. Any state secret, in or related to, such as diplomatic stuff, intelligence agency, military, weapon research or production, etc.

2. Act as a password manager. Use one master password and this software to manage all other passwords. This is the recommended practice of using this software. Because, in order to achieve sufficient password strength, each password must be long and complex, which must be difficult to remember. Therefore, using a master password and a password manager will greatly simplify the difficulty of memorizing.

3. Various secret files stored on the local computer. In this way, in case your computer is hacked or stolen, only the encrypted file will be stolen, your secret will remain safe.

4. Secret information that needs to be transmitted through public channels (such as e-mail), or stored online in facilities provided by commercial services (such as online disks, cloud files).

## Features

1. Three algorithms (AES256, Serpent, Twofish) are used in tandem. Even if two of them have weaknesses or vulnerabilities, the final result is still safe. AES256 is a mainstream algorithm, and the other two are also well-known open source algorithms.  
Theoretical analysis on the strength of multi-level cascaded encryption, [Bellare and Rogaway's paper](https://eprint.iacr.org/2004/331.pdf) shows:
  >"Double encryption is no less securer than its least secure component."  
  >"Triple-encryption vastly improves security over single or double encryption."

2. The encryption strength can be up to 2 ^ 768, or 10 to the 231th power. In contrast, the strength of the mainstream Aes256 algorithm is only 10 to the 77th power. Generally speaking, the weakness of a algorithm will reduce its strength. However, in the case of 10 ^ 231, even if all the above three algorithms have weaknesses, the overall strength is still very sufficient.3. Use non-parallel encryption modes and special scheme to maximize cracking cost. It is designed such that inner layer can't be tried before outer layer is fully carried out (entire content, rather than a block of content). The leads to an outcome that bigger files encrypted with this are more difficult to crack, e.g. a file of 16 MB length has a crack cost of 3 millions times more than that of a 16 bytes file.

3. Non-parallel encryption mode is used, and a specially designed multi-layers scheme is used, such that it is impossible to even start inner layer cracking before the outer layer decryption has been computed completely.  
  
    The common encryption mode often allows the decryption to be performed in parallel and block by block, both practices reduce the encryption strength. One block is usually merely 16 bytes long, so it takes a lot less for the attacker to complete one trial with a 16-bytes long block than with the whole body of a big file.  
  
    Using the specially designed scheme of this software, the larger the file is, the more difficult it is to be cracked. For example, a 16 MB file is 3 million times more difficult to crack than a 16 byte file.

4. Do not provide any oracle to the attacker. Oracle (a famous one, the padding oracle) can significantly reduce the encryption strength. For example, the strength could be reduced from multiplication to addition, such as from 256 * 256 to 256+256,

5. Unicode characters can be used in password, such as Chinese, Korean and Arabic characters. Common encryption tools require that password characters be letters, numbers, or symbols. The use of Unicode characters opens another channel for passwords. You can enter a long sentence in your native language as a password. This sentence usually has a special meaning for you. Therefore, it not only increases the password strength, but is also easier to memorize.  
  
    The best password is a mixture of Unicode characters, uppercase and lowercase letters, numbers, and symbols.
  
    For Aes256, the full strength password is a string consisting of uppercase and lowercase letters/numbers/symbols with a length of 40. A Unicode character in the password is split into two ascii characters for use and can be counted as two ascii characters.

6. The number of salting loop is adaptively selected to enhance the encryption strength for short passwords. (Note that it is not recommended to rely on salting for encryption strength. You should try to use longer and more complex passwords. It is for those who do not follow the recommendation, I provide this nice function.)
  
    For Aes256, the length of its full strength password is 40. The password of length 40 is difficult to remember and use. People like or are used to using short passwords, this is by human nature and is almost unchangeable. As a result, the strength of encryption is often seriously reduced in practical applications.
  
    For example, if 6 letters/numbers/symbols are selected as the password, the total number of different combinations is only~2 ^ 38, which is about 2.7 * 10 ^ 12. The simple brutal-force cracking is a way that tries all possible combinations. Even the floating point operation speed of the common modern-day PC has reached 10 ^ 12/s, it can quickly try out all combinations for such a password, let alone today's top computers, which has floating point operation speed at 10 ^ 20/s.
  
    For this issue, a method called salting is invented. Salting is a method of recursively computing hash of a message. The original password is used to calculate a hash, and then the hash of the previous hash, repeatedly for a number of loops, and the last hash value is used as the password, in place of the original password. Salting is used to redistribute the original password. The original password is concentrated in a small region, which can be easily traversed in brutal-force cracking. After redistribution, the passwords are randomly scattered in the password space determined by the entire password length (for example, 2 ^ 256). In this way, the cracker has to either traverse the entire password space, which is usually large and impossible to complete, or limit his attempts to the original password space region. however, for each password to be tried, he has to go through the process of salting again. If the number of salting loop is large, it will consume a lot of computing resource, which increases the cost of trying a single password, thereby increasing the overall encryption strength.
  
    For example, suppose that it takes 10 ^ -9 seconds (1 nanosecond) to try a single password in brutal-force cracking. If the number of salting loop is 10 million, the salting process takes 1 second, which is equivalent to 10 ^ 9 times increase in password strength, or 4.6 increase in password length. If the original password length is 10, salting can make the password length go up to 14.6, which can almost resist the brutal-force cracking of modern-day top computers for one year. In summary, salting reduces the user's labor of memorizing passwords and entering long passwords.
  
    With salting used, and assuming password is composed of uppercase and lowercase letters/numbers/symbols, for modern computing power, the recommended safe password length is at least 10. If Unicode (such as Chinese characters) characters are mixed in the password, it will be more secure.
  
    Adaptive salting is to appropriately change the number of salting loops according to the computer hardware speed and the password length you enter.

## How to use the software

I declare that, to the best of my knowledge, this software does not contain viruses and trojans. However, since it is used for encryption purposes, users should proceed with caution, including:

1. After downloading the software, verify the hash value of the file.

2. And/or use a sandbox environment, such as various virtual machines, to prevent * * * in case * * * this software contains viruses, it will not infect your main environment. Or the software can be scanned for viruses and certified to be virus free (see the third party verification section).

3. When encrypting and decrypting with this software, you should disconnect your PC from the network in case this software or other software in the environment contains trojans/backdoors, steal your important secrets and send them out through the network.

## How to obtain

The temporary price: US$300 per person use license, volume price is negotiable. You can contact me by private message on this platform for purchasing.

## File Hash

The hash of the file is used to verify the integrity of the file and that it has not been tampered with. In Windows, the tool used for this purpose is fciv.exe Before using fciv.exe, you should verify that its digital signature is correct.

V1.0:

## Environment

This software currently only works in Microsoft Windows environment. The required operating system is Windows 8.1 or above, and Microsoft .Net Framework 4.5.1 or above should have been installed.

## Disclaimers

If you do not agree with the following terms, please do not use this software. To the best of my knowledge, this software does not contain viruses and trojans. This software has the characteristics, functions or/and capabilities described in this article. However, I do not guarantee with 100% certainty. If the software does contain defects, or my view and judgment are wrong, and the customer is damaged as a result, I can at most compensate as much as the price of the software. I do not assume any responsibility for customer losses caused by illegal or improper use of this software.

## install

If it fails to run, it may be that your environment is missing some DLL files provided by the operating systems. You can contact me to help to solve the problem.

At present, only English and 中文(Chinese) version is available. If your need other language version, contact me.

## Third party verification

1. To verify that the software does not contain viruses, method: Back up your computer environment, install and use the software, and after a period of time, compare the files with those in the backup. There should be no unknown or unexpected changes between the two set.

2. To verify that this software does not contain trojans, backdoors, and data theft through the network, method: In a test and controlled environment, use this software while monitoring and logging network traffic, and no abnormal network traffic should be observed.

3. View source code: source code is not provided, but you can arrange to view it.

The update service is free for life.

Special requirements and customized services

For example, if you want to select other encryption algorithm as the underlying algorithm, I may provide customization services for you.

**Contact**

