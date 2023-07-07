# Giveaway-Script
## Description
Single winner giveaway script with variable timer &amp; 60 second claim conformation. Duration of giveaway based on argument from start command. If winner doesn't claim in 60 seconds, it draws another winner. Once claimed, it shuts down. Can be forced to stop by permissions. Uses !enter, !claim, !giveaway start {#}, !giveaway end, !ga start {#} !ga end as its command syntax, please make sure you disable any of those before you install this.

# Things to note
  * Before installing, please rename or disable any command that uses the following syntax
    * !giveaway
    * !ga
    * !enter
    * !claim
    * !leave
# Usage
  !giveaway start {#} - starts the giveaway based on the number (in minutes) you provide
  
  !ga start {#} - alternative to !giveaway start
  
  !giveaway end - forces the giveaway to stop
  
  !ga end - alternative to !giveaway end
  
  !enter - enters the name of the user who used the command
  
  !claim - claims the prize

  !leave - allows user to remove themselves from the current giveaway
  
  # How it works
  Streamer or moderator triggers the start command to start a giveaway for the number of minutes you want it to run. Contestants enter using the !enter command. At the end of the time given, the bot will chose randomly from the list of contestants (assigned by role). If contestant who wins claims the prize by using the !claim command, the script will end and reset everything for the next giveaway. If the contestant who is chosen by the bot does not use the !claim command within 60 seconds, the bot will chose another person and remove the original winner from the list of contestants. If there is no one left to issue the !claim command, it will stop the script and reset it self for the next giveaway.
