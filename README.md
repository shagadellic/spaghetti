------------------------------------------------------------------------------------------------------------
Create conditions based charge automation to top up EV from home solar & battery
------------------------------------------------------------------------------------------------------------

example- start charging the car when there is '4 kw' solar and the home battery is at 100%

example- stop charging the car when the is '0 kw' solar and home battery is at 60%

Car will automatically top up off peak if required (normal charge setting for me)
40% of home battery is usually enough for my daily commute

Could use the data to control all sorts of guff...

----------------------------------------------------------------------------------------------------------
miner.ps1 - collects data into an sqlexpress database.
----------------------------------------------------------------------------------------------------------

I have had to fudge my own 'API' as the vendor will not grant me access to theirs (atm..)

Edit the config.xml file to connect to your solar vendors web gui - tested with Chrome

Use find_page_title.ps1 to find the site title to put into config.xml

Add your authenticated tokenised URL to the <URL> field

update the fields with the line number you want to retrieve (copy your solar gui page 
  
and paste to notepad, count line number starting at zero)
  
This all runs well on a preloved (<150 bucks) Intel Nuc siting in the laundry
                                       
Was fun to circumvent server side Java that snookered the usual powershell html parsing                                        

If you have a powerwall you are probably laughing at the need for this ;)
                                       
----------------------------------------------------------------------------------------------------------
WIP - UI to select conditions to start / stop charging etc
----------------------------------------------------------------------------------------------------------

Unofficial API for Tesla is available from https://www.teslaapi.io/

App use db data to determine start / stop etc based on parameters entered

Initial testing has not bricked my car. Use at your own peril. 

Going to Run the UI on tablet that is stuck on my kitchen wall.. using it as a home hub  

----------------------------------------------------------------------------------------------------------

If you have the cash, just buy more panels and a bigger battery - dont worry about active management ;)

Twitter: @psanders_aus

