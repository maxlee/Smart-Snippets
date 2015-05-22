## Smart Snippets for Sublime Text 2/3

### Installation on Sublime Text 2 and Sublime Text 3

#### Mac/Linux Instructions

1. CD into Sublime Text packages folder

    `cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages`

  or

    `cd ~/Library/Application\ Support/Sublime\ Text\ 3/Packages`

2. Clone repository into packages folder

`git clone https://github.com/maxlee/Smart-Snippets.git`

#### Windows Instructions

`cd "%AppData%\Sublime Text 3\Packages\User"`
`git clone https://github.com/maxlee/Smart-Snippets.git`


### Installation on Package Control

#### <a href="https://sublime.wbond.net/installation">How to install Package Control</a>
Get Package Control for Sublime Text 2/3. Installation is through the Sublime Text 2/3 console. The console is accessed via the ctrl+` shortcut or the View > Show Console menu. Once open, paste the appropriate Python code for your version of Sublime Text into the console.

##### SUBLIME TEXT 2
```
import urllib2,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')
```
##### SUBLIME TEXT 3
```
import urllib.request,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

1. Package Control: Add Repository `https://github.com/maxlee/Smart-Snippets`
2. Package Control: Install Package `Smart Snippets`
3. Restart ST2/3 editor

### “Help! My snippets doesn’t work anymore in HTML/CSS files!”

By default, Emmet overrides Tab key behaviour and expands its own abbreviations instead native snippets. You can either disable this feature in user preferences (add `"disable_tab_abbreviations": true` setting into your _Settings — User_ file) and use `Ctrl+E` or `Ctrl+Alt+Enter` to expand Emmet abbeviations or move your snippets to Emmet as described [here](https://github.com/sergeche/emmet-sublime/issues/16#issuecomment-8427268). I’m investigating possibility to expand native snippets via Emmet Tab key handler.

### Thank you for installing Smart Snippets. Enjoy coding!
![DemoCSSVideo](https://raw.githubusercontent.com/maxlee/Smart-Snippets/gh-pages/img/css.gif)
![DemoHTMLVideo](https://raw.githubusercontent.com/maxlee/Smart-Snippets/gh-pages/img/html.gif)

### APIs

Trigger          | Property
:--------------- | :-----------:
html + tab       | HTML Default Template
aitms + tab      | a href=itms-apps://
bgc + tab        | background-color:
bd + tab         | border: ${1:1px} dotted ${2:transparent}
bd- + tab        | border: ${1:1px} dashed ${2:transparent}
bd. + tab        | border: ${1:1px} dotted ${2:transparent}
bdn + tab        | border: 0 none
! + tab          | !important
cur + tab        | cursor: pointer
f + tab          | font: 12px/1.5 Tahoma, sans-serif
ffyh + tab       | font-family: "Microsoft YaHei"
ext + tab        | @extend
inc + tab        | @include
mix + tab        | @mixin
imp + tab        | @import "${1}"


