# Card Count 🃏

A simple **card counting practice program** written in C.  
It allows you to enter card values and keeps track of the running count based on basic Blackjack card counting rules.  

---

## 📖 How it works
- The program asks for a card name (`2–10`, `J`, `Q`, `K`, `A`, or `X` to exit).  
- It assigns a value to the card:  
  - `J`, `Q`, `K` → **10**  
  - `A` → **11**  
  - Numbers `2–10` → their respective value  
- It then adjusts the **count** using the following rules:  
  - `2–6` → **+1**  
  - `10, J, Q, K` → **-1**  
  - Others → **0** (no change)  
- Entering `X` exits the program.  

---

## 🚀 Usage

1. Compile the program:

```bash
   gcc card_count.c -o card_count
```

2. Run it:

```bash
./card_count
```
3. Input card names one by one. Example:

```text
Enter the card_name:
5
Current count: 1

Enter the card_name:
K
Current count: 0

Enter the card_name:
X
```
---
## 🛠 Example session

```text
Enter the card_name:
4
Current count: 1

Enter the card_name:
10
Current count: 0

Enter the card_name:
A
Current count: 0

Enter the card_name:
X
```
---
## 📌 Notes

- Invalid inputs (e.g., Z or numbers outside 1–10) will show:

```text
i dont understand that value!
```

- The counter starts at 0 and updates as you enter card values.
