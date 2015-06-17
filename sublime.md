1. 安装Sublime3或2，百度云盘
2. 安装ctrl+` Package Control https://packagecontrol.io/installation
    Sublime3
    import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
    Sublime2
    import urllib2,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')
3. 安装Markdown语法包https://packagecontrol.io/packages/MarkdownEditing
    Install Sublime Package Control
    From inside Sublime Text, open Package Control's Command Pallet: CTRL SHIFT P (Windows, Linux) or CMD SHIFT P on Mac.
    Type install package and hit Return. A list of available packages will be displayed.
    Type MarkdownEditing and hit Return. The package will be downloaded to the appropriate directory.
    Restart Sublime Text to complete installation. Open a Markdown file and this custom theme. The features listed above should now be available.
4. 