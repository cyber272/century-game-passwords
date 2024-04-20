# # Century Game Passwords and SSH Connection Guide.

---
## SSH Connection Guide

To connect to each Century level using SSH, use the following command format:
```bash
ssh century(N)@century.underthewire.tech
```
Replace `(N)` with the level number (e.g., Century0-1, Century1-2, etc.).

When prompted, enter the corresponding password from the table below to access the specified Century level.

## Encrypted Passwords

The passwords have been encrypted for security. To access the encrypted passwords file, please refer to [**`Century_file`**](signed_encrypted_century.asc).

## Usage

1. **Clone this repository to your local machine**:
   ```bash
   git clone https://github.com/cyber272/century-game-passwords.git
   ```

2. **Decrypt the passwords file**:
   - Ensure you have GPG installed on your system.
   - Use the following command to decrypt the passwords:
     ```bash
     gpg --decrypt signed_encrypted_century.asc > decrypted_passwords.txt
     ```
   - Enter your GPG passphrase when prompted to decrypt the file.

3. **Use the decrypted passwords**:
   - Open `decrypted_passwords.txt` to view the passwords for each Century level.
   - Use these passwords when connecting via SSH to the respective Century level.

## Public Key

To decrypt the passwords, use the following [**GPG_Public_Key**](Sam-pubkey.gpg):
```
<Sam-pubkey.gpg>
```

For more details on GPG encryption and usage, refer to the [GPG Documentation](https://www.gnupg.org/documentation/).

---

### Additional Notes
- **SSH Security**: Always verify the authenticity of the SSH server before entering passwords.
