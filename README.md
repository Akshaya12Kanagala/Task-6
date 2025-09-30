# Task-6:  Create a Strong Password and Evaluate Its Strength.

### Objective: Understand what makes a password strong and test it against password strength tools.
### Tools: passwordmeter.com

### Step 1 : Creating Passwords
We start with a very simple password and gradually improve it by adding complexity.<br>
 Example:   <br>               
`password123`        -    Common word + numbers (weak, dictionary vulnerable)  <br>
`Password123!`	     -    Added uppercase + symbol (better but still predictable) <br>
`Pa$$w0rd2025!`      -	  Substituted letters with symbols, added year (medium strength) <br>
`!QwErTy2025#`	     -    Random case + numbers + symbol (stronger, less predictable) <br>
`9$TgH@1!pLk#2025Zz` -    Long, random mix of all character types (very strong) <br>

### Step 2 : Testing Passwords
Using https://passwordmeter.com, the results were:<br>
`password123` → Weak  <br>
Short length, dictionary word, predictable. <br>
`Password123!` → Medium <br>
Includes uppercase and symbol, but still guessable. <br>
`Pa$$w0rd2025!` → Medium/Strong  <br>
Substitutions help but attackers often try these patterns. <br>
`!QwErTy2025#` → Strong <br>
Longer, mixed characters, unpredictable. <br>
`9$TgH@1!pLk#2025Zz` → Very Strong <br>
High complexity, length, and randomness.

### Step 3 : Best Practices Learned
1.  Use at least 12–16 characters.
2.  Mix uppercase, lowercase, numbers, and symbols.
3.  Avoid dictionary words and common substitutions (Pa$$w0rd is weak).
4.  Use random strings or passphrases for memorability.
5.  Do not reuse passwords—consider a password manager.

### Step 4 : Common Password Attacks
1. **Phishing** — Tricks users (via fake emails/sites) into handing over credentials; relies on human error. Example: a fake PayPal email forces a user to log in on a cloned site so the attacker steals the real credentials. If passwords are reused, the attacker can access multiple accounts.
2. **Credential stuffing** — Attackers reuse stolen username/password pairs across many services to find reused credentials. It exploits humans tendency to reuse passwords, check compromises with haveibeenpwned.com.
3. **Brute force attacks** — Automated programs try every possible character combination until the password is found. They often start with very common passwords (e.g., 123456, password) and can factor in site rules; 80%+ breaches involve these techniques and attackers sometimes bypass attempt limits.
4. **Dictionary attacks** — A targeted form of brute force that tries common words/phrases (and their variations). More advanced versions use personalized info (pet names, bands) scraped from social profiles.
5. **Password spraying** — Attackers try a few very common passwords against thousands/millions of accounts (instead of many guesses on one account). This avoids lockout detection and often targets SSO/cloud platforms at scale.
6. **Keylogger attacks** — Malware or physical devices record every keystroke, capturing passwords, usernames, security answers, and credit-card numbers. Delivered via phishing, drive-by downloads, or trojans; once installed they’re hard to detect — prevention is critical.
7. **Man-in-the-Middle (MitM) attacks** — An attacker intercepts and relays communications between user and service (often via a proxy). They can present a fake login page, capture credentials as the user types, then use those credentials live on the real site while the victim sees normal behavior.
8. **Rainbow table attacks** — Attackers use precomputed tables of plaintext-to-hash mappings to reverse hashed passwords quickly. Since systems store hashes, a rainbow table can crack common hashing algorithms fast; such tables/tools (e.g., RainbowCrack, 0phcrack) and precomputed sets are available on the dark web.

### Step 5 : Summary
Password complexity + length = stronger security. <br>
Weak passwords fall quickly to brute force and dictionary attacks.<br>
Strong passwords combine randomness, length, and mixed characters.<br>
