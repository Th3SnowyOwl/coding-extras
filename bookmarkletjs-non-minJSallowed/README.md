### How To Code This

### Line 1-3;    
You don't even need to change this
### Line 4 
find `<input type="text"` in the source code of the website you want to login to, you want to use the `name=""` value, change the `USERNAME_SOURCE_NAME` value in our code to `name=""` from the html the `<input type=text` username form, do not change `name*=` and put your username/email in the `YOUR_USERNAME_HERE` spot.
### Line 5
find `<input type="text"` in the source code of the website you want to login to, you want to use the `name=""` value, change the `PASSWORD_SOURCE_NAME` value in our code to `name=""` from the html the `<input type=text` password form, do not change `name*=` and put your password in the `YOUR_PASSWORD_HERE` spot.
### Line 6
This is the most complicated line to change, so go to the website you want to login to, and press: "CTRL+u" or whatever you keyboard shortcut is to open the source, open a text editor or if you don't have that you can use an online editor, I recommend `https://editpad.org`, paste the code from `login.txt` in, go back to the source tab and search for `login` or `submit` if you find some code (usually next to the login and password stuff), find: `name=""` and replace it for `SUBMIT_BUTTON_NAME`, in the same line of text in the source code, there should be a value that says `id=""` use this value to replace `SOURCE_BUTTON_ID`, DON'T TOUCH ANY OF THE OTHER CODE.
### Finishing 
When you are done coding this, make all this code one line, delete the space behind `var` in line one, repeat this process for each line, 
`spaces are allowed between single lines of code but there should not be spaces in front of `{` or `;` and copy your finished code and save it as a bookmark.`
### Example of compacted code, you need to compact it to use it as a bookmarklet.
`javascript:(function(){var d=document;s=d.querySelector;s.call(d,'input[name*=user_id]').value='jondoe12345';s.call(d,'input[name*=password]').value='password12345';s.call(d,'button[id*=submit],input[type=button][id*=submitbutton],.button').click();}())`
