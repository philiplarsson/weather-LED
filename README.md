# Weather polling LED

So I wanted to build a small thing that tells me whether I should bring rain clothes or not. And of course learn some python and raspberry pi.

The script is run as a cron job each 30 minutes.
```bash
*/30 * * * * python /home/pi/weather.py
```

The script then gets the weather info from SMHI's [API](http://www.smhi.se/klimatdata/oppna-data/meteorologiska-data).

After the weather data is collected it does some blinky stuff to display that new data have been collected and then checks the following 8 hours for any rain/snowfall. A red LED is turned on if the weather is *bad* and a green LED is turned on if the weather is *good*.

# Pictures
Prototype
![Prototype](https://raw.githubusercontent.com/philiplarsson/weather-LED/master/img/prototype.jpg)

Soldering
![Soldering](https://raw.githubusercontent.com/philiplarsson/weather-LED/master/img/soldering.jpg)

Finished
![Finished](https://raw.githubusercontent.com/philiplarsson/weather-LED/master/img/finished-product.jpg)


