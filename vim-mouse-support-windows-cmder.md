## Enable mouse support in Windows cmder Vim

###Use cases
* When you're using  mouse in the first place (e.g. editing PPT/Word) and need a quick glance at your code
* Resize split, click tabs, scroll through code quickly etc


Make sure you have the following setting for vim:
* set mouse=a
* set ttymouse=xterm2. Refer http://usevim.com/2012/05/16/mouse/
* set nocompatible

And for cmder setting
* Keys & Macro --> Control --> Mouse options: [x] Send mouse click event to console
* Keys & Macro --> Control --> Mouse buttons actions: [x] Buffer only
* Keys & Macro --> Mark/Copy --> Select text with mouse
  * Remove vim.exe from the exceptions, it it's there
  * Add modifier for text selection (e.g. Ctrl) to activate for text selection with left-mouse click, if you need this feature
  * And try disable the 'Intelligent mode' if split resize using mouse is a bit quirky





