
<center><img src="http://currentconfig.com/images/tp_diag01.gif" alt="Underneath is for savages!" style="width:95%; height:95%"/></center>

While probably as conentious as the debate over the question of horizontal toilet paper dispensing orientation, there is really only one answer when asked what the proper level of indentation is for proper python coding...4 spaces!
Note that this is spaces and not tabs.  Below I highlight how to setup a couple of the most popular editors (emacs users are a lost cause anyways) for four (4) space tab emulation.

<center><img src="/blog/images/nedit_tab_stops.png" alt="Emulating Tab Stops"/></center>

### Nedit
<pre>
Preferences -> Default Settings -> Tab Stops…
  Recall to 'Save Defaults...' after making your changes.
</pre>
### VIM
<pre>
  :set expandtab         insert space characters whenever the tab key is pressed
  :set tabstop=4         to insert 4 spaces for a tab
  :retab                 to change all the existing tab characters to match the current tab settings
  :set shiftwidth=4      to change the number of space characters inserted for indentation
</pre>
To aid in training yourself to adhere to this methodology, I recommend adding the *-tt* switch to your python2 alias in order to 
elevate inconsistant tab usage warnings to full-blown errors.  Thankfully, python3 helpfully errors out when you mix tab and spacing
indendation without the requirement that you recall to add any extra switches.
