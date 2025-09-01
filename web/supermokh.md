# SuperMokh
![WhatsApp Image 2025-08-30 at 15 28 26_276f3bf2](https://github.com/user-attachments/assets/57338117-1ef8-49af-8da0-1def19a7f3e9)

- Open inspect, there is a comment inside HTML. It looks like a base64 encryption.

![WhatsApp Image 2025-08-31 at 11 33 37_f83cd154](https://github.com/user-attachments/assets/e2944252-d820-4159-8c46-5daa2c72d878)

- Decrypt the data, and it will show the username and password.

![WhatsApp Image 2025-08-30 at 15 32 50_a822ad9b](https://github.com/user-attachments/assets/fd7478fb-2293-4590-bcb2-63cabf0ff0c0)

After logging in, it will show a flag, but it can't open because it uses a guest account.

![WhatsApp Image 2025-08-30 at 15 27 40_7306b28f](https://github.com/user-attachments/assets/dc4a596d-c59d-4205-bf17-b33c0196955d)

Modify the URL from `/dashboard.php` to `/flag.php`, it says only SuperMokh can have the flag access. So now we know the admin username is SuperMokh.

<img width="1916" height="869" alt="image" src="https://github.com/user-attachments/assets/9a3a2e92-15b4-4ff2-9ebb-17c7c55bb7d6" />

- Go back to `dashboard.php` and inspect the cookie, the value of `auth_token` looks like JWT token.

<img width="1739" height="814" alt="image" src="https://github.com/user-attachments/assets/6a28f650-5815-46b8-bb41-b671f7432a80" />

- Then I decode the JWT token, so the webpage uses the role and username. We can modify that to fit the admin token.

<img width="1738" height="824" alt="image" src="https://github.com/user-attachments/assets/350b95d5-ce58-4892-bd2c-3f5f06e7f5e7" />

- I then encode the modified data into a new JWT token. Copy and then replace the value of `auth_token` with the new token. Then click the view flag.

<img width="1690" height="964" alt="image" src="https://github.com/user-attachments/assets/2f473416-7e0a-4613-a66a-989a233cfede" />

- Flag: 3108{m0kht4r_d4h4r1_l3g3nd_n3v3r_d13s}

### Lessorn learned
- Always inspect the cookie.
- I learned from others' write-ups that it's more efficient to handle JWT tokens with Linux.

