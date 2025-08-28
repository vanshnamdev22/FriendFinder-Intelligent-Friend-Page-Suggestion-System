# FriendFinder+: Intelligent Friend & Page Suggestion System

FriendFinder+ is a **Python-based social graph analysis tool** that takes your social network data, cleans it, and generates **smart friend and page recommendations** using mutual connections and shared interests.  

This project uses a sample dataset (`data.json`) containing **30 users** and **27 community pages** with detailed friend and interest connections.  

---

## 🚀 Features

- 🧹 **Data Cleaning**
  - Removes users with missing names
  - Removes duplicate friends and pages
  - Filters out inactive users

- 👥 **Friend Recommendations**
  - Suggests friends based on **mutual friends**
  - Ranks suggestions by mutual connection count

- 📄 **Page Recommendations**
  - Suggests pages based on **shared interests** with other users

- 📊 **Easy to Extend**
  - Ready for graph visualization (e.g., `networkx`, `matplotlib`)

---

## 📂 Project Structure

```
📁 FriendFinder+
│
├── data.json                    # Original dataset with users & pages
├── cleaned_codebook_data.json   # Cleaned dataset (auto-generated)
├── friendfinder.py              # Main Python script
└── README.md                    # Documentation
```

---

## 🛠️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/friendfinder-plus.git
cd friendfinder-plus
```

Ensure **Python 3.8+** is installed.  
No external libraries are needed (uses built-in `json` module).

---

## ▶️ Usage

Run the program:

```bash
python friendfinder.py
```

### What happens:

1. Loads data from `data.json`
2. Cleans and saves it as `cleaned_codebook_data.json`
3. Displays all users, their friends, and liked pages
4. Shows **friend** and **page** recommendations for a sample user (default `user_id = 1`)

---

## 🔍 Example Output

```
Data cleaned and saved to 'cleaned_codebook_data.json'.

Users and Their Connections:

Amit (ID: 1) - Friends: [2, 3, 4, 5, 6] - Liked Pages: [101, 102]
Priya (ID: 2) - Friends: [1, 3, 4, 5, 6, 7] - Liked Pages: [102, 103]
...

Pages:
101: Python Developers
102: Data Science Enthusiasts
103: AI & ML Community
...

People You May Know for User 1: [7, 8, 9, 10, 11, ...]
Pages You Might Like for User 1: [103, 104, 105, 106, ...]
```

---

## 🧩 How It Works

1. **Data Cleaning:**
   - Deduplicates friend lists and page records
   - Removes invalid or empty entries

2. **Friend Recommendation Algorithm:**
   - Builds a **graph of users**
   - Counts **mutual friends**
   - Suggests top-ranked friends

3. **Page Recommendation Algorithm:**
   - Finds users with **similar liked pages**
   - Suggests new pages the target user hasn’t liked yet

---

## 🔮 Future Improvements

- 📈 Graph visualization of relationships
- 🤖 ML-based recommendation ranking
- 🌐 Web interface for friend/page suggestions
- 🔍 Interest-based clustering

---

## 🤝 Contributing

Contributions are welcome!  
Fork this repo, create a branch, and submit a pull request.

---

## 📜 License

This project is licensed under the **MIT License**.

---

