Day 29: Hands-On Cryptography with VeraCrypt

What is VeraCrypt?
VeraCrypt is an open-source disk encryption software used to create encrypted virtual drives or encrypt entire storage devices (like USB drives) or system partitions.

What it does and How it works:

Function: It protects data by creating an encrypted "container" (a file) that acts as a secure virtual disk. When this container is mounted with the correct password, it appears as a new drive on your computer. All files saved to this drive are automatically encrypted. When unmounted, the drive disappears, and the container file remains encrypted and inaccessible without the password.

The Process: It uses a user-defined password to generate a strong encryption key. This key is used to scramble all data written to the container using a chosen algorithm (like AES).

Key Features Explored:

Volume Types: Can encrypt files (containers), non-system partitions, or entire systems.

Hidden Volume: A advanced feature that allows you to create a second, secret volume within the free space of another encrypted volume. This provides "plausible deniability" if you are forced to reveal a password, as there is no way to prove the hidden volume exists.
