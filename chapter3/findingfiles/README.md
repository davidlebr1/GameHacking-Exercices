# Finding Files

In this exercice we have to find the file that store the high score. We will use Process Monitor to find the file. 

With some filter, I found that the file is : `C:\Users\David\AppData\Local\Temp\gh_hs_p.dat`

## Bonus

In bonus we need to change the highscore to a big value. When I open the file with notepad we don't see much. There is probably more in it because when we do `cat -A gh_hs_p.dat` we see some blank space and other wierd ascii value. 

With Sublime Text we can see hex value. For a 30 points we have this `1f00 0000` and `1e` is equal to Record Separator in ASCII. Let's change to `1e00 0000`. Yes, now we have 31 points. Max ascii hex value is `7f`. So, let's try `7f7f 7f7f`.

Cool, the high score is now 2139062143 
