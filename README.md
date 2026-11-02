# Penetrative Library Search Assistant

The library website uses TinyFish web search to find resources and book
recommendations based on a reader's interests, favorites, and recently viewed
books. TinyFish credentials stay in the local Python server and are never sent
to the browser.

## Setup

1. Install Python 3.11 or later (required by the TinyFish SDK).
2. Install the dependencies:

   ```powershell
   python -m pip install -r requirements.txt
   ```

3. Set `TINYFISH_API_KEY` in `.env` to your TinyFish API key. If `.env` does not exist,
   copy `.env.example` to `.env` first. Keep `.env` private; do not commit or
   share it.
4. Start the library website:

   ```powershell
   python main.py
   ```

5. Open <http://127.0.0.1:5000> in your browser and choose **AI Assistant**
   from the menu.

Search results are live web results and may link to books that are not in the
library inventory. The server binds to localhost; keep it running while using
the website. TinyFish Search is subject to its account's rate and usage limits.
