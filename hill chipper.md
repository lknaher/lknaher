You want to calculate the Hill cipher encryption using the key matrix \( K \) and plaintext values \( p1 = 9 \) and \( p2 = 20 \).

### Key Matrix \( K \):
\[
K = \begin{pmatrix}
11 & 8 \\
3 & 7
\end{pmatrix}
\]

### Plaintext Vector \( P \):
\[
P = \begin{pmatrix}
p1 \\
p2
\end{pmatrix}
=
\begin{pmatrix}
9 \\
20
\end{pmatrix}
\]

### Encryption Formula:
The ciphertext is calculated using matrix multiplication:
\[
C = K \times P \mod 26
\]

### Step 1: Matrix Multiplication
Multiply the key matrix \( K \) by the plaintext vector \( P \):

\[
C = \begin{pmatrix}
11 & 8 \\
3 & 7
\end{pmatrix}
\times
\begin{pmatrix}
9 \\
20
\end{pmatrix}
=
\begin{pmatrix}
(11 \times 9) + (8 \times 20) \\
(3 \times 9) + (7 \times 20)
\end{pmatrix}
=
\begin{pmatrix}
99 + 160 \\
27 + 140
\end{pmatrix}
=
\begin{pmatrix}
259 \\
167
\end{pmatrix}
\]

### Step 2: Take Modulo 26
Now, take each element of the result mod 26:

\[
C = \begin{pmatrix}
259 \mod 26 \\
167 \mod 26
\end{pmatrix}
=
\begin{pmatrix}
259 \mod 26 = 25 \\
167 \mod 26 = 11
\end{pmatrix}
\]

### Step 3: Convert Numbers to Letters
The numbers 25 and 11 correspond to the letters:
- 25 = Z
- 11 = L

### Final Result:
The Hill cipher encryption of the plaintext vector \( P = (9, 20) \) using the key matrix \( K = \begin{pmatrix} 11 & 8 \\ 3 & 7 \end{pmatrix} \) gives the ciphertext **"ZL"**.
