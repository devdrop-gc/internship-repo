# 🔒 Password Strength Evaluation

## 🎯 Objective
Understand what makes a password strong and test it against password strength tools.

## 🛠️ Tool Used
- https://www.passwordmeter.com (The Password Meter)

---

## 📝 Tested Passwords & Results
| Password                     | Length | Score | Verdict      | Key Feedback                                   |
|-------------------------------|--------|-------|-------------|-----------------------------------------------|
| password                     | 8      | 8%    | Very Weak    | Lowercase only; repeated/consecutive letters |
| Password123                  | 11     | 75%   | Strong       | Mixed-case + numbers; predictable sequences  |
| p@ssw0rd2025!                | 13     | 100%  | Very Strong  | Random letters, numbers, symbols; minor repeats |
| BatteryHorse99!!             | 16     | 100%  | Very Strong  | Long mixed-case with numbers/symbols; some repeats |
| CorrectHorseBatteryStaple    | 25     | 90%   | Very Strong  | Long letters-only; many consecutive lowercase |
| K9$mZv!qL2&wP8^eJ9#xT        | 21     | 100%  | Very Strong  | Long random mix of all char types             |

📸 Full screenshots available in `/screenshots`.

---

## 💡 Key Learnings & Best Practices
1. **Length is the #1 factor** – longer passwords are exponentially harder to crack.
2. Passphrases (4+ random words) are more secure and easier to remember than complex short passwords.
3. Avoid dictionary words, names, dates, and common substitutions (like p@ssw0rd).
4. Minimum recommended: **16+ characters** with mixed types.
5. Use a password manager + enable 2FA everywhere.

---

## 🕵️‍♂️ Common Password Attacks Researched
- **Brute Force**: Tries all possible combinations – defeated by length.
- **Dictionary Attack**: Uses common word lists + patterns – avoided with randomness.
- **Hybrid Attack**: Combines dictionary with rules (e.g., adding "123!") – countered by unique, non-patterned structures.

---

## 📊 Summary
The evaluation shows that length and randomness trump forced complexity. A simple passphrase like `CorrectHorseBatteryStaple` outperforms short "secure" passwords in both strength and usability.
