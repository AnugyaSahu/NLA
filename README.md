
- Here are some of my python code for:
1. QR with classical gram-schmidt orthogonalisation process

1. **Start with Matrix \( A \)**: Begin with your original matrix \( A \) that you want to decompose.
2. **Orthogonalize Columns**: For each column in \( A \), subtract out parts that align with previously processed columns to make it perpendicular to them.
3. **Normalize Columns**: Scale these new columns to have a length of one, creating the orthogonal matrix \( Q \).
4. **Form Upper Matrix \( R \)**: Use the projections and scalings to fill in the corresponding entries of the upper triangular matrix \( R \).
5. **Complete Process**: Repeat these steps for all columns in \( A \) to get the matrices \( Q \) and \( R \) such that multiplying \( Q \) and \( R \) gives back \( A \).

3. QR via householder reflector
4. QR via Givens rotation process

<!---
:)
--->
