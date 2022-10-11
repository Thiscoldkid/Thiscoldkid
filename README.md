- 👋 Hi, I’m @Thiscoldkid
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Thiscoldkid/Thiscoldkid is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
{
    "manifest_version": 2,
    "name": "Blooket Cheat Extension",
    "description": "Made by OneMinsraft2#5394 | Blooket extension based off: https://github.com/glixzzy/blooket-hack along with more cheats",
    "author": "OneMinesraft2#5394",
    "version": "6.9.0",
    "permissions": [
        "tabs",
        "webRequest",
        "webRequestBlocking",
        "debugger",
        "<all_urls>"
    ],
    "background": {
        "scripts": [
            "background.js"
        ],
        "persistent": true
    },
    "content_scripts": [
        {
            "matches": [
                "*://*.blooket.com/*"
            ],
            "js": [
                "content.js",
                "jwt-decode.js"
            ]
        }
    ],
    "browser_action": {
        "default_popup": "popup.html",
        "default_title": "Blooket Hack"
    },
    "web_accessible_resources": [
        "*ata.js",
        "scripts/*",
        "css/*"
    ],
    "icons": {
        "1024": "icons/1024.png"
    }
}
Footer
