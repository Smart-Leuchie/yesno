# ComBoard — Setup Guide

## 1. Get the file onto the iPad

Recent iPads increasingly won't open a local `.html` file straight into a full Safari page — tapping it in Files/iCloud usually just shows a static preview, and even the Share sheet and Split View drag-and-drop tricks that used to work around this don't always appear anymore. If that's what you're running into, skip straight to **Option B** below — it takes about 10 minutes once and then always just works.

**Option A — direct, if your iPad allows it:** Send `ComBoard.html` to the iPad any way that's convenient (AirDrop, email, iCloud Drive/OneDrive) and tap it. If it opens as a normal Safari page with an address bar, great — go to step 2. If it only shows a preview/the raw code, or Safari never appears as an option to open it with, use Option B instead.

**Option B — host it at a proper web address (recommended, more reliable):**

This puts the same file on a free, permanent web address so the iPad just visits it like any other website — no local-file quirks, and it still works offline after the first visit since everything runs on the device from then on.

1. On a computer, go to **github.com** and create a free account if you don't already have one (just an email, username and password — no payment details needed).
2. Click the **+** in the top-right corner → **New repository**. Name it `comboard`, leave it set to **Public**, then click **Create repository**.
3. On the new repository's page, click **Add file → Upload files**, then drag in the `index.html` file (attached to this conversation — it's the same ComBoard app, just renamed so the web address comes out clean). Click **Commit changes**.
4. Go to the **Settings** tab of the repository → **Pages** (left-hand menu) → under "Build and deployment" set Source to **Deploy from a branch**, Branch **main**, folder **/(root)**, then **Save**.
5. Wait about a minute, then refresh that Pages settings screen — it will show your live address, something like `https://yourusername.github.io/comboard/`.
6. On the iPad, open **Safari** and type that address in. It should load exactly like the app you've already seen. From here, carry on with step 2 below (Add to Home Screen).

Because the repository is public, the blank app code is publicly viewable at that address — but that's just the empty template. None of the actual pictures or words you add on the iPad are stored in that code; they stay only in that iPad's own local storage, so nothing personal ever goes online. If you'd rather this not be publicly visible at all, GitHub also offers private repositories with Pages on paid plans, or your organisation's own web hosting (if it has any) would work exactly the same way — just upload `index.html` there instead and use whatever address it gives you.

## 2. Add it to the Home Screen (so it behaves like an app)

1. With the page open in Safari, tap the **Share** icon (square with an arrow).
2. Tap **Add to Home Screen**.
3. Give it a name (e.g. "ComBoard") and tap **Add**.
4. Launch it from the new icon on the Home Screen — it will open full-screen, without Safari's address bar.

From now on, always open it from the Home Screen icon rather than a browser bookmark, so it stays in the same "installed" context and its saved tiles are always there.

## 3. How the board is laid out

There are three rows above the main picture grid:

- **Quick row** — always-visible shortcut tiles (Please, No, Don't know, Understood, Yes, Excuse me by default). Tap one and it speaks just that word, on its own, nothing else.
- **Category row** — the "verb" of the sentence: Like, Want, Have, Do, Need, See. Tap one to choose it.
- **Intensity row** — six strengths from "---" (strongest negative, dark red) through "-"/"+"  to "+++" (strongest positive, dark green). Tap one to choose how strongly it's put.

Tapping a picture in the grid then finishes the sentence: it speaks the chosen category+intensity phrase, followed by the picture's own word. For example: Like + "+" + a photo labelled "dinner" → "I like dinner". Need + "++" + the same photo → "I really need dinner". Want + "--" + a photo labelled "a drink" → "I don't want a drink". One shared set of pictures works with every category and every intensity, so you only add each picture once.

**A note on the intensity wording**: I've set sensible starting phrases for each of the six strengths (e.g. for "like": --- "I really don't like", -- "I don't like", - "I don't really like", + "I like", ++ "I really like", +++ "I really really like"). Have a look at these in Settings once the board's in use — some phrasings across six categories inevitably read a little oddly for certain words (e.g. "I really do" or "I really have"), and you can reword any of them freely.

## 4. Add your first tiles

- Press and **hold the title bar** at the top (about 2 seconds) to enter **Edit mode**. There's no visible edit button in normal use, so this won't happen by accident. While in Edit mode, the category and intensity rows are hidden (they're not needed for adding pictures) and the quick row and main picture grid both become editable.
- **For the quick row**: tap the **+** at the end of the quick row, choose a photo (optional) and type the word (e.g. "Yes"). These are spoken exactly as typed, with no prefix.
- **For the main grid**: tap the **+** tile. Choose a photo, and type just the item/action itself (e.g. "dinner", "a drink", "the toilet") — not a full sentence, since the category and intensity supply that part.
- **Tip — name your photos first and skip typing altogether**: if the text box is still empty when you pick a photo, ComBoard fills it in automatically from the photo's file name (underscores and hyphens become spaces, and spaces in a file name work exactly as you'd expect — "a drink.jpg" becomes "a drink"). So if you rename a folder of photos on a computer first (e.g. "dinner.jpg", "a drink.jpg", "the toilet.jpg") and pick them via the **Files** browser rather than the Photos library, each one fills itself in and you just tap Save. This only works reliably when picking from Files — photos picked straight from the Camera Roll usually keep an unhelpful name like "IMG_1234.HEIC", so for those you'll still want to type the wording yourself. Either way, whatever gets filled in stays fully editable before you save.
- Tap **Save**.
- Tap any existing tile while still in Edit mode to change its picture or wording, or to delete it.
- Tap **Done** (top right) to leave Edit mode and go back to normal use.

## 5. Settings

While in Edit mode, tap **Settings** to:
- Rename the board.
- Turn tile text labels on/off.
- **Categories & intensity** — rename any category word, add a new category (e.g. "feel"), delete one you don't need, or edit the exact phrase spoken at each of the six strengths for any category.
- Choose a different built-in voice, and adjust speech rate/pitch.
- **Export Board** — saves a backup file (pictures, categories, quick row and settings) you can keep safe or load onto another iPad.
- **Import Board** — loads a backup file, replacing everything currently on the board.

## 6. Set up Guided Access (locks the iPad to this app)

1. On the iPad: **Settings → Accessibility → Guided Access** → turn it **On**.
2. While there, set a **passcode** for Guided Access (separate from the iPad's own passcode) — this is what's needed to exit later.
3. Open ComBoard from the Home Screen icon.
4. **Triple-click the side/top button** to start Guided Access.
5. You can circle any area of the screen to disable touch there if needed, then tap **Start** (top right).
6. To exit later: triple-click the button again and enter the Guided Access passcode, then tap **End**.

Everything the board needs (images, tiles, speech) is stored on the iPad itself and works without an internet connection once the page has been opened at least once.

## Notes

- The app speaks using the iPad's own built-in system voice (the same speech engine used by VoiceOver/Speak Screen), so no extra voice download or setup is needed.
- Photos are automatically resized to keep the board fast and use less storage — no need to resize photos yourself first.
- If you ever need to reset from scratch, use **Import Board** with a blank/backup file, or delete tiles individually in Edit mode.
