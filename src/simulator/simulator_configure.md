![](https://wiki.threefold.io/img/tf_tde_intro.png)

# Simulator for the ThreeFold Grid and Token

[webixexample](simulator_configure_webix.html ':include :type=iframe width=100% height=300px frameBorder="0" scrolling="no" align="center"')

- Growth: is in nr of nodes which we expect the grid to have in 5 years
    - 1% marketshare of current internet cloud is about 5-10.000.000 servers.
- Token Price: 
    - you can select a fixed nr, eg. 3 would mean you expect the TFT token price to go to 3 USD over 5 years.
    - you can also select auto, then the price will be ```valuation of grid (which is 30 months over revenue) / nr of TFT on the network```
    - when ```auto``` we call the TFT price calculated the TFT Index.
- Unit Price Range: these are the sales prices of the cloudunits, this param allows you to choose the avg price range the grid will sell it capacity for (more info see [here](cloud_units_4.md))
    - CU = compute unit, 15 USD is a good price (on market between 20 and 200)
    - SU = storage unit, 10 USD is a good price (on market between 20 and 160)
    - NU = network unit
- The simulator only takes capacity sales into consideration, the TFT will be used for many other usecases but this has not been included in the simulator. The simulator is just a way how to visualize the growth of the grid in relation to TFT price and how the TFGrid provides a good economical model for the TF Farmer.

All the results of the simulator are an export from the simulator which is part of our SDK, there are more then 450 combinations exported, we hope you like it.

If you are a python enthusiast you can use the simulator yourself see: [getting started with simulator yourself.](farming_simulate.md) . You will need some familiarity with Python & Jupyter.

