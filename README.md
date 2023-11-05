# RSA Factoring Challenge

## Author - Kevin Kipkoech

### RSA (cryptosystem)

Developed in the 1970s RSA-(Rivest-Shamir-Adleman) is a public key cryptosystem though one of the oldest to date as its been used widely over the internet for secure communications using a secure socket layer(SSL). 

Its an asymemetric public-private key crptosystem in which the public key can be known by everyone and is used for encryption. The private key is known by only the owner and is used for decryption. Both keys are different.

It is very difficult to factorize large numbers and thus this is it depends for its security, sounds good, using the problem as a way to secure itself.

#### How it works:

1. Choose two large prime number, p and q. Then compute n = pq. n is known as the modulus
2. The totient of n is then computed 
3. Then choose an integer e such that 1 < e < n(totient) and gcd(e, n(totient)) = 1. e is the public exponent and is used to encrypt the message.
4. compute d such that ed = 1 mod totient(n). d is called the private exponent and it is ed to decyrpt the message.

<please refer to this for further understanding>

https://jaredatandi.hashnode.dev/rsa-factoring
https://en.wikipedia.org/wiki/RSA_(cryptosystem%29



A public key cryptosystem that is used to secure data transmission, though one of the oldest so far but it’s used widely:triumph:.
The acronym RSA come from the surnames of Ron Rivest, Adi Shamir and Leonard Adleman who publicly described the algorithm in 1977.
In this case the encryption is public and  distinct from the decryption key, which is kept private. An RSA user creates and publishes a public key based on two large prime number, along with an auxiliary value. The prime numbers are kept secret. Messages can be encrypted by anyone, via the public key, but can only be decoded by someone who knows the prime numbers.
RSA is a very versatile algorithm and is one of the most widely used public-key algorithms to date. However, RSA is not without its weaknesses:skull:.
The biggest weakness of RSA is that it is vulnerable to attack if the private key is compromised. This is why it is important to keep the private key secret and to use a good quality random number generator to generate the keys. Another weakness is the it is relatively slow compared to other public-key algorithms
:skull:.
### For the ALX task
0. Factorize all the things!

Factorize as many numbers as possible into a product of two smaller numbers.
•	Usage: factors <file>
o	where <file> is a file containing natural numbers to factor.
o	One number per line
o	You can assume that all lines will be valid natural numbers greater than 1
o	You can assume that there will be no empy line, and no space before and after the valid number
o	The file will always end with a new line
•	Output format: n=p*q
o	one factorization per line
o	p and q don’t have to be prime numbers
o	See example
•	You can work on the numbers of the file in the order of your choice
•	Your program should run without any dependency: You will not be able to install anything on the machine we will run your program on
•	Time limit: Your program will be killed after 5 seconds if it hasn’t finish
•	Push all your scripts, source code, etc… to your repository
o	we will only run your executable factors
1. RSA Factoring Challenge
RSA Laboratories states that: for each RSA number n, there exist prime numbers p and q such that
n = p × q. The problem is to find these two primes, given only n.
This task is the same as task 0, except:
•	p and q are always prime numbers
•	There is only one number in the files
