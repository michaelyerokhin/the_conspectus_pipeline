# The Conspectus

This repo houses the ingestion/parsing layer of The Conspectus infrastructure. It will handle fetching, normalizing, and updating data from curated sources.

# 🗓️⚙️ Technical Roadmap
<img width="569" height="838" alt="image" src="https://github.com/user-attachments/assets/d0aa7e40-4a53-4cb9-996d-34dbfdc5c3cd" />

👉👉 View/comment on the design decisions [here](https://www.notion.so/Technical-Design-Decision-Document-28b250e4573880e7bf67dc5d701b48cf?source=copy_link).

---

## Steps

1. Clone and enter the repo
   
   ```bash
   git clone https://github.com/michaelyerokhin/the_conspectus_pipeline
   cd the_conspectus_pipeline
   ```

2. Create and activate a virtual environment

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate    # macOS/Linux
   .\.venv\Scripts\activate  # Windows PowerShell
   ```

3. Install dependencies and the package (editable)

   ```bash
   cd src/
   pip install -r requirements.txt
   pip install -e .
   ```

4. Test it (in /src)...

   ```bash
   python -m ingestion.main
   ```

   You should see:

   ```
   Running ingestion pipeline...
   ```

---

## 🧰 Notes

- `.venv/` is your local environment — it’s ignored by Git.
- Add new dependencies with (for example, I did):

  ```bash
  pip install black
  pip freeze > requirements.txt
  ```

- BTW, let's format our .py files after coding:

  ```bash
  black .
  ```
