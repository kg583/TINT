TINT Package v1.1 Info

TINT, or TI Number Theory, is a package of lists and programs designed for number theoretic computation and analysis on the TI-83+ series of calculators.
These programs are designed to be used as subprograms for larger projects, and are optimized for numbers less than 10^14.
TINT's main feature is the precomputation of many arithmetic properties of a given input number stored for later use (e.g. number of divisors, totient function, etc.).

To install, simply download and open the group TINT. All TINT programs are denoted by θNT followed by 2 or 3 characters.
The following variables and lists are defined for an input N after executing the program θNTN.
Most programs also require the factorization of N to be defined via θNTN (exceptions are noted below).

Updated in v1.1
-Removed all remainder( commands to allow support for older OS's
-Added primality/probable prime tests (see documentation for θNTPT)
-Added Lucas sequence generation (see documentation for θNTLS)
-Added more numerical properties to θNTIS
-Adjusted variable allocation for less shuffling (most inputs that are "bases" are now θ instead of Q)
-Better edge case support
-General bug fixes

Vars
Properties
-W: # of distinct prime divisors
-O: # of prime divisors
-C: Compositeness
-T: # of Divisors
-S: Sum of Divisors
-A: Aliquot sum
-B: Abundance
-H: Totient
-L: Liouville function
-U: Mobius function
-R: Radical
-D: Arithmetic derivative
-G: Log arithmetic derivative

Inputs
-N: Number
-M: Arbitrary whole number (usually a modulus)
-P: Arbitrary whole number (usually a prime)
-Q: Arbitrary whole number
-K: Input number (usually small)
-θ: Input number (usually a base)

Program Vars
-X: Bound
-Y: Loop var
-Z: Counter

Empty Vars
-E: Empty var
-F: Empty var
-I: Empty var
-J: Empty var
-V: Empty var

Lists
-P: Prime factors of N
-A: Prime multiplicities of N
-B: A+1 (useful for divisor-related queries)
-D: Divisors of N
-E: Divisor multiplicities of N
-U: Unitary divisors of N (those divisors with multiplicity 1)

Premade Lists
-P100: All primes < 100
-P1000: All primes < 1000

Programs (return is Ans unless otherwise stated; if a return is also stored in a variable, it is denoted in parentheses)
-NTCL: List of integers between 1 and N coprime to N --> L1; v1.1
-NTCM: Carmichael's function of N
-NTCQ: Ramanujan's sum of N base Q
-NTCR: Core of N mod M
-NTDK: Sum of Kth powers of divisors of N (K=0 <--> # of Divisors, K=1 <--> Sum of Divisors)
-NTET: Euler's totient function of N (w/o known factorization); v1.1
-NTFP: Find the smallest prime factor of N (w/o known factorization)
-NTGCD: GCD of L1
-NTIS: If N satisfies property; input the property as a two-letter string from the list below in Ans; tests may not always return 1 for a positive result
--"CM": Carmichael
--"LC": Lucas-Carmichael
--"KP": K-Perfect (K=2 <--> Perfect)
--"GI": Giuga
--"SF": Squarefree
--"KS": K-Smooth
--"KR": K-Rough
--"PW": Perfect power
--"AB": Abundant
--"PF": Powerful
--"UN": Unusual
--"RF": Refactorable
--"SP": Semiprime
--"NH": Nonhypotenuse
--"AP": Almost perfect
--"KH": K-Hyperperfect
--"HP": Hemiperfect
--"BL": Blum
--"RG": Regular
--"HD": Harmonic divisor
--"AR": Arithmetic
--"PP": Primary pseudoperfect
--"KA": K-Almost prime (K=1 <--> Prime, K=2 <--> Semiprime, K=3 <--> Sphenic); v1.1
--"CK": Coprime to K; v1.1
--"PR": N has primitive roots; v1.1
--"θR": θ is a primitive root modulo N; v1.1
--"SH": Sphenic; v1.1
-NTJK: Jordan's totient of N base K
-NTLCM: LCM of L1
-NTLI: Intersection of L1 and L2 --> L3
-NTLJ: Kronecker symbol (generalized Legendre/Jacobi symbol) of N base θ (--> Z)
-NTLS: Establish Lucas sequences U(P,Q) & V(P,Q) --> u & v (respectively); v1.1
-NTMO: Multiplicative order of θ mod M
-NTMU: Mobius function of N (w/o known factorization)
-NTMX: θ^K mod M (modular exponentiation algorithm)
-NTN: TINT data initialization for N
-NTPF: Prime factorization of N; does not preserve N
-NTPG: List of primes up to X --> L1
-NTPN: Generate next prime given all previous primes in L1
-NTPT: If N is prime (w/o known factorization); v1.1: input the test as a two-letter string from the list below in Ans; a trial divison by 2 is always performed; tests may not always return 1 for a positive result
--"TD": Trial division (all odd integers from 3 to √N)
--"AD": Accelerated trial division (3, all integers ±1 mod 6 from 5 to √N)
--"PD": Prime trial division (all primes from 2 to √N)
--"Fθ": Fermat probable prime test base θ
--"FR": Fermat probable prime with random base
--"Sθ" or "MR": Strong probable prime test base θ (also called the Miller-Rabin primality test)
--"SR": Strong probable prime test with random base
--"Eθ": Euler probable prime test base θ
--"ER": Euler probable prime test with random base
--"LU": Lucas probable prime test for parameters P & Q
--"LS": Strong Lucas probable prime test for parameters P & Q
--"LS": Extra strong Lucas probable prime test for parameters P & Q
--"BP": Baillie-PSW primality test
--"FB": Frobenius probable prime test for parameters P & Q
--"FI": Fibonacci probable prime test
--"PL": Pell probable prime test
-NTRL: List of primitive roots modulo N --> L1; v1.1
-NTVP: Multiplicity of P in N (--> Z)

Have any questions? Found a bug?
Contact kg583 on TI-Basic Developer.

Copyright © Kevin Gomez 2018. All rights reserved.
