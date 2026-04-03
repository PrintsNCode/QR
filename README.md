# Free Dynamic QR with GitHub Pages

Simple project to create a **100% free dynamic QR code** using GitHub Pages. The idea is very simple: the QR always points to the GitHub Pages URL, and you only change the destination inside `index.html` when you want to update the target.

## How it works

1. The QR points to:
   
   ```
   https://printsncode.github.io/QR/
   ```

2. That page contains a redirect:

   ```html
   <meta http-equiv="refresh" content="0; url=https://example.com">
   ```

3. When you change that URL and commit, the QR destination changes without regenerating the QR.

## Advantages

- 100% free
- No subscriptions
- No tracking platforms required
- Works forever (as long as GitHub Pages exists)
- Editable from mobile or computer
- Instant updates
- No backend required

## How to change the destination

### From mobile (GitHub app or browser)

1. Open the repository
2. Open `index.html`
3. Press edit
4. Change the URL
5. Commit changes

### From computer

Edit this line:

```html
<meta http-equiv="refresh" content="0; url=https://your-new-link.com">
```

Commit and done.

## Project structure

- `index.html` → Main redirect (production)
- Test HTML files → Experiments
- QR generator page → Helper tool

## Use cases

- Instagram bio QR
- Business cards
- Stickers
- 3D printed QR plates
- Posters
- NFC alternatives

## Limitations

- No analytics (unless added manually)
- Small delay after commit (GitHub Pages deploy time)

## Possible future improvements

- Optional click tracking
- Multiple redirects
- Simple UI editor
- Password protected links

## License

Free to use. No warranty.
