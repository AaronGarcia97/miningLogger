# Mining Logger
by [Aaron](https://github.com/AaronGarcia97)

Script designed in order to track profit from dwarfpool pool using ethereum
miner. :chart_with_upwards_trend: :moneybag:

### Instructions
- Go to root directory `cd /path/to/miningLogger`
- Open your terminal and type `echo "YourWalletAddress" > wallet.txt`
- Give the script permission of execution `chmod +x miningLogger`
- Test that the script works `./miningLogger`

#### IMPORTANT
Unless you want to run the code manually every certain amount of time,
you have to setup a cronjob to tell the script to execute every X hours.

- Open your terminal
- Type `crontab -e`
- Insert in 1st line `SHELL=/bin/bash`
- Insert a 2nd line depending on when you want to run the file in my case I want
  the script to be ran at 00:00 every day. So I insert:
  <br>`0 0 * * * /path/to/miningLogger`
- Save the file and close it,
  <br>Vi editor `ESC -> !wq -> ENTER`
  <br>Nano editor `CTRL + X -> Y -> ENTER`

#### More info:
[crontab](https://www.debian-tutorials.com/crontab-tutorial-cron-howto)<br>
[vi editor](https://kb.iu.edu/d/adxz)<br>
[nano editor](https://wiki.gentoo.org/wiki/Nano/Basics_Guide)<br>


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

Feel free to contribute to the project. More features coming soon. :octocat:

#### DONATIONS
ETH: 0xd6ab25cda715df49d0fb64d5fa4752fc46265f98
