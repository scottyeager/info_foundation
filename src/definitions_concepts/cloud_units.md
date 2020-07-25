## Cloud Units

![](cloudunits_abstract.png)
Cloud units are the way to account for farmed and used capacity. Cloud units are the compute, storage and network equivalent to kWh - kilowatt-hour - the unit of energy.

We use three categories of units:

- Compute: the amount of data processing power, specified as the number of virtual CPU cores (logical [CPUs](https://en.wikipedia.org/wiki/Central_processing_unit)) and RAM ([Random Access Memory](https://en.wikipedia.org/wiki/Random-access_memory))
- Storage: the size of data storage capacity
- Network: the amount of data that travels in and out of the acquired storage units or data that travels to/from compute capacity expressed in GB.

Its a very easy way how to express capacity.

- The TF Certified Farmers can define the price per CU,SU,NU.
- When a solution gets requested, it always gets converted to required amount of CU,NU,SU required.

### Cloud Units (v4)

In this table you find all you need to know to how we calculate cloud units on the ThreeFold Grid.
v4 is the one used in summer 2020 on TFGrid 2.2+

| CU (Compute Unit) = MRU/CRU per month  |   |   |   | |
|---|---|---|---|---|
| GB Memory         |  4  | 8  |  2  | = MRU |
| nr vCPU           |  2  | 1  |  4  | = CRU |
| Passmark Minimum  | 500  | 250 | 1000 | is performance cpu |

Passmark is not measured in the grid, we only use resource units to calculate the su & cu. Passmark is a CPU benchmark. Passmark used in simulators and as checking mechanism to make sure we have enough performance per CU.


| SU (Storage Unit) = MRU/SRU per month | HD (HRU)  |  SSD (SRU) |  
|---|---|---|
| GB Storage Capacity  |  1000  | 100  | 

| NU (Network Unit = per GB) = NRU per month | GB (NRU)  | 
|---|---|
| GB transfered OUT or IN  |  1  |



### link to resource units

!!!include:resource_units_table
!!!include:resource_units_calc_cloud_units


### Some Examples of CU and SU in Detail

#### Compute Unit (CU): 

- 4 GB memory & 2 virtual CPU 
- Recommended price on TF Grid = 10 USD
- Market price = between 40 USD and 180 USD

#### Storage Unit (SU):

- 1TB of neto usable storage (1000 HRU)
- Recommended price on TF Grid = 10 USD
- Market price = between 20 USD and 200 USD


> Its good to compare how the suggested sales prices compare with the market, [see here](cloud_pricing.md)