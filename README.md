
- Here are some of my python code for:
1. QR with classical gram-schmidt orthogonalisation process

- **Start with Matrix \( A \)**: Begin with your original matrix \( A \) that you want to decompose.
- **Orthogonalize Columns**: For each column in \( A \), subtract out parts that align with previously processed columns to make it perpendicular to them.
- **Normalize Columns**: Scale these new columns to have a length of one, creating the orthogonal matrix \( Q \).
- **Form Upper Matrix \( R \)**: Use the projections and scalings to fill in the corresponding entries of the upper triangular matrix \( R \).
- **Complete Process**: Repeat these steps for all columns in \( A \) to get the matrices \( Q \) and \( R \) such that multiplying \( Q \) and \( R \) gives back \( A \).

2. QR via householder reflector

- **Initialization**: Start with the matrix \( A \) that you want to decompose.
- **Form Householder Reflector**: For each column, create a Householder reflector, which is a special matrix that can zero out all elements below the diagonal in a column.
- **Apply Reflector**: Apply the Householder reflector to the current column and to all columns to the right, transforming the current column into a vector with zeros below the diagonal.
- **Accumulate Reflectors**: Store each reflector so that when applied in sequence, they form the orthogonal matrix \( Q \).
- **Extract \( R \)**: The transformed matrix becomes the upper triangular matrix \( R \), and the product of all reflectors gives the orthogonal matrix \( Q \), resulting in \( A = QR \).
3. QR via Givens rotation process

- **Initialization**: Start with matrix \( A \) that you want to decompose.
- **Identify Elements to Zero**: Focus on each element below the diagonal that you want to zero out.
- **Apply Givens Rotation**: For each target element, create a Givens rotation, which is a rotation in the plane of two coordinates designed to zero out the chosen element.
- **Update Matrix**: Apply the Givens rotation to the entire matrix \( A \), progressively zeroing out the lower triangular part to form the upper triangular matrix \( R \).
- **Accumulate Rotations**: The product of all Givens rotations forms the orthogonal matrix \( Q \), resulting in \( A = QR \).

<!---
:)
--->
