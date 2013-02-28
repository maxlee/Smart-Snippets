## About
LEGO Snippets in Sublime Text 2

http://coffeehtml.com

## How to install

1. Package Control: Add Repository `https://github.com/maxlee/LEGO-Snippets`
2. Package Control: Install Package `LEGO Snippets`
3. Restart ST2 editor

### “Help! My snippets doesn’t work anymore in HTML/CSS files!”

By default, Emmet overrides Tab key behaviour and expands its own abbreviations instead native snippets. You can either disable this feature in user preferences (add `"disable_tab_abbreviations": true` setting into your _Settings — User_ file) and use `Ctrl+E` or `Ctrl+Alt+Enter` to expand Emmet abbeviations or move your snippets to Emmet as described [here](https://github.com/sergeche/emmet-sublime/issues/16#issuecomment-8427268). I’m investigating possibility to expand native snippets via Emmet Tab key handler.