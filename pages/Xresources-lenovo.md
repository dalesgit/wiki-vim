!#include "/home/dale/bin/Xresources-themes/light/raven-light.Xresources"
!#include "/home/dale/bin/Xresources-themes/light/one-light.Xresources"
!#include "/home/dale/bin/Xresources-themes/light/Tomorrow.Xresources"
!#include "/home/dale/bin/Xresources-themes/light/raven-light.Xresources"
!#include "/home/dale/bin/Xresources-themes/light/iterm-AtomOneLight.Xresources"
#include "/home/dale/bin/Xresources-themes/light/PaperColor.Xresources"
!#include "/home/dale/bin/Xresources-themes/xcolors-simple_rainbow.Xresources"
!#include "/home/dale/bin/Xresources-themes/xcolors-zenburn.Xresources"
!#include "/home/dale/bin/Xresources-themes/xcolors-Visiblue.Xresources"
!#include "/home/dale/bin/Xresources-themes/base16-atelier-estuary-256.Xresources"
!#include "/home/dale/bin/Xresources-themes/base16-atelier-forest-256.Xresources"
!#include "/home/dale/bin/Xresources-themes/base16-atelier-lakeside-256.Xresources"
!#include "/home/dale/bin/Xresources-themes/base16-github-256.Xresources"
xterm*VT100.Translations: #override \
                 Ctrl Shift <Key>V:    insert-selection(CLIPBOARD) \n\
                 Ctrl Shift <Key>C:    copy-selection(CLIPBOARD)
! ! Allow sixel graphics. https://github.com/hackerb9/lsix
xterm*decTerminalID:	vt340
! window size?
!xterm*geometry: 86x23
! Use a nice truetype font and size by default... 
!xterm*faceName: DejaVu Sans Mono Book
!xterm*faceName: NotoSanMono-Medium
!xterm*faceName: SourceCodePro 
!xterm*faceName: Inconsolata
xterm*faceName: JetBrains Mono 
!xterm*faceName: icons-in-terminal 
xterm*faceSize: 12
