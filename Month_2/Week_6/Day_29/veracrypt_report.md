VeraCrypt Exercise Report

Objective: To gain practical experience with on-disk encryption by creating and using a VeraCrypt encrypted file container.

Steps Performed:

Installation: Downloaded and installed the VeraCrypt software.

Volume Creation: Initiated the Volume Creation Wizard and selected "Create an encrypted file container."

Volume Type: Chose a "Standard VeraCrypt volume" (over a hidden one).

Location & Name: Created a folder named "Containers" and saved the volume as Container1.

Encryption Settings: Selected the default encryption algorithm (AES) and hash algorithm (SHA-512).

Volume Size: Allocated a 1 GB size for the container.

Password & Keyfiles: Created a strong password. Noted the software's warning for weak passwords.

Formatting & Randomness: Formatted the volume. The software collected random data from my system, including mouse movements, to strengthen the encryption keys. I moved the mouse randomly until the indicator turned green, signaling sufficient entropy.

Mounting & Use: Selected a virtual drive letter (A:), clicked "Mount," selected my Container1 file, entered the password, and successfully accessed the 1GB encrypted drive.

Testing: Copied a file into the mounted Z: drive to verify functionality. Unmounted the drive, confirming the file was inaccessible until remounted with the password.

Key Learning & Incident:
The exercise successfully demonstrated the core principle of virtual encrypted disks. A key practical lesson was learned about data management: I accidentally lost a file by deleting the container while the file was inside it. This reinforced the critical concept that the container is a secure data store, and its deletion is equivalent to physically destroying a drive. Luckily, it was a recoverable file, making it a valuable, low-stakes lesson.