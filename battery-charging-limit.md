# Battery threshold
setting up a battery threshold is best way to preserve battery lifespan , especially if you leave it plugged in while using .
## Testing
first we need to check your battery name and apply the limit for once to check if the inbuilt service of the laptop kernel is working 
```bash
ls sys/class/power_supply
```

this command lists *power-supply* devices connected to your laptop

here you will find your battery name mostly `BAT0` OR  `BAT1`

Asus hardware controllers can only accept the thresholds of `40 , 60 , 80 and 100`

