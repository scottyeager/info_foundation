# Cloud Units (v4)

In this table you find all you need to know to how we calculate cloud units on the ThreeFold Grid.
v4 is the one used in summer 2020 on TFGrid 2.2+

| CU (Compute Unit) = MRU/CRU per month  |   |   |   | |
|---|---|---|---|---|
| GB Memory         |  4  | 8  |  2  | = MRU |
| nr vCPU           |  2  | 1  |  4  | = CRU |
| Passmark Minimum  | 500  | 250 | 1000 | is performance cpu |

| SU (Storage Unit) = MRU/SRU per month | HD (HRU)  |  SSD (SRU) |  
|---|---|---|
| GB Storage Capacity  |  1000  | 100  | 

| NU (Network Unit = per GB) = NRU per month | GB (NRU)  | 
|---|---|---|
| GB transfered OUT or IN  |  1  |


Passmark is not measured in the grid, we only use resource units to calculate the su & cu. Passmark is a CPU benchmark.

Passmark used in simulators and as checking mechanism to make sure we have enough performance per CU.

## Resource Units

- cru = 1 logical core of CPU 
- mru = 1 GB of memory
- hru = 1 GB of storage capacity on a harddisk
- sru = 1 GB of storage capacity on a SSD

Resource units are measured on the hardware

## Resource Units To Cloud Units

### su

basically 1 SU is 1 TB of HD capacity, or 100 GB of SSD capacity with a buffer of 20%.

```python
su = (hru / 1000 + sru / 100 / 2) / 1.2
```

### cu

Basically 1 CU is 2 vcpu with max oversubscription on cpu core of 4 and min required mem is 4GB. Oversubscription of 4 is still gentle we know that many other providers use more.

```python
cu = min((mru - 1) / 4, cru * 2)
```


## Some Examples of CU and SU in Detail

### Compute Unit (CU): 

- 4 GB memory & 2 virtual CPU 
- Recommended price on TF Grid = 10 USD
- Market price = between 40 USD and 180 USD

### Storage Unit (SU):

- 1TB of neto usable storage (1000 HRU)
- Recommended price on TF Grid = 10 USD
- Market price = between 20 USD and 200 USD


> Its good to compare how the suggested sales prices compare with the market, [see here](cloud_pricing.md)