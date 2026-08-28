# Discord Downloader

Download the images and messages from the Discord conversation currently open in your browser.

> This is an independent project. It is not affiliated with, endorsed by, or supported by Discord.

## Free and unlimited

Discord Downloader is completely free to use. It has no subscriptions, paywalls, accounts, usage tracking, or extension-imposed download limits. The amount of content you can export depends only on the chat history your Discord account can access and what Discord makes available in the open conversation.

## Features

- Export an open Discord DM, group DM, or channel as an offline HTML archive.
- Export only messages with uploaded image attachments, retaining the image, caption, sender, and timestamp.
- Download all detected uploaded image attachments in one ZIP file.
- Name downloads after the current conversation or channel.
- Walk upward through the chat to collect the history available to your signed-in account.

## Install

1. Download `DiscordDownloader-v1.0.0.zip` from the [latest release](../../releases/latest).
2. Extract the ZIP to a permanent folder on your computer.
3. Open `chrome://extensions` in Google Chrome.
4. Turn on **Developer mode** in the top-right corner.
5. Select **Load unpacked**.
6. Choose the extracted folder that contains `manifest.json`.

## Use

1. Open the Discord conversation or channel you want to export at [discord.com](https://discord.com).
2. Click the **Discord Downloader** extension icon.
3. Choose one of the available actions:

   - **Export full chat as ZIP** — creates a ZIP with `index.html` and an `images` folder.
   - **Export image messages as ZIP** — includes only messages with Discord-uploaded image attachments, along with their captions and metadata.
   - **Download all images as ZIP** — creates one ZIP containing the detected image attachments only.
4. Choose where Chrome should save the downloaded file.

Extract an HTML export and open `index.html` in any modern browser.

## Privacy and permissions

The extension reads only the Discord conversation already open in your signed-in browser tab. It does not use Discord's API, send messages, edit content, upload your chat data, or transmit information to an external service.

It requests these Chrome permissions solely to perform the export:

- `activeTab` — access the Discord tab you explicitly export.
- `downloads` — save your selected archive.
- `scripting` — reconnect to a Discord tab that was already open when the extension was loaded.

## Limitations

- Only history available to your Discord account can be exported.
- Deleted, inaccessible, or unavailable content cannot be recovered.
- Image-specific exports intentionally exclude Discord UI imagery, emoji, stickers, avatars, and link-preview artwork; they include Discord uploaded attachments.
- Very large conversations may take time to load and export.

## License

Licensed under the [MIT License](LICENSE).
