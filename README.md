# Mining Logger
by Aaron

Script designed in order to track profit from dwarfpool ethereum
miner.

### Instructions
- Go to root directory `cd /path/to/miningLogger`
- Open your terminal and type `echo "YourWalletAddress"` > wallet.txt
- Give the script permission of execution `chmod +x miningLogger`
- Test that the script works `./miningLogger`

#### HINT
Unless you want to run the code manually every certain amount of time,
you have to setup a cronjob to tell the script to execute every X hours.

- Open your terminal
- Type `crontab -e`
- Insert in 1st line `SHELL=/bin/bash`
- Insert a 2nd line depending on when you want to run the file in my case I want
  the script to be ran at 00:00 every day. So I insert:
  `0 0 * * * /path/to/miningLogger`
- Save the file and close it,
  if using vi ESC -> !wq -> ENTER
  if using nano CTRL + X -> Y -> ENTER

More info on cron [here](https://www.debian-tutorials.com/crontab-tutorial-cron-howto)

The script prints a `log.txt` that looks like this:

```
0.27713078                    <- previous balance
0.277131
2018-05-24 00:00:00
-----------------------------
0.28366063                    <- current balance
0.00652985                    <- this is the difference (current-previous)
2018-05-25 00:00:00
-----------------------------
```

ENJOY!

Feel free to contribute to the project. More features coming soon.

#### DONATIONS
ETH: 0xd6ab25cda715df49d0fb64d5fa4752fc46265f98
