Settings for Sublime Text3

Packages:

Packege Control: 
https://packagecontrol.io/installation#st3

Put this in View > Show Console menu

    import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; 
    pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener(     urllib.request.build_opener( urllib.request.ProxyHandler()) ); 
    by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), 
    please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by) 

Emmet:

    Open Command Palette in Sublime Text
    Pick “Install Package” command
    Find and install “Emmet” plugin
    
SideBarEnhancements:   

    Open Command Palette in Sublime Text
    Pick “Install Package” command
    Find and install “SideBarEnhancements” plugin
    
Add tab validation to .rb files for 2 spaces instead of 4

 To limit this configuration to Ruby files, first open up a Ruby file in the editor, and then go to Preferences -> Settings -> More -> Syntax Specific -> User. This should open a settings window named Ruby.sublime-settings
    
     {
       "tab_size": 2,
       "translate_tabs_to_spaces": true
     }
