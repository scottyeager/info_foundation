## Farming Logic (year 2020)

- Farming is calculated once a month, at the fist day of the next month.
    - executed by opensource minting (farming) code
    - all the proof of capacities are stored on a redundant storage system and hashed 
    - these hashes verify the authenticity of the report
- 4 days later the TFT are being transferred to the farmer.
    - the [grid_council](grid_council) needs to vote on the minting
    - the code is automatically executed using our Farming Bots but needs verification from the council before execution can happen
- the minting code will create & distribute the TFTv1 (till end 2020)
    - in transaction message the hash will be stored which is link to the proof of the capacity for each minting operation

> DISCLAIMER: ThreeFold Foundation organizes this process. This process is the result of the execution of code written by opensource developers (zero-os and minting code) and a board of 9 people (grid_council) who check this process voluntarily. No claims can be made or damages asked for to any person or group related to ThreeFold Foundation like but not limited to the different councils.

### Minting Rules V2.0 (starting May 2020)

## Maximum amount of TFT

There will be a maximum amount of 4 billion TFT minted.

## Cloud production Rate (CPR)

The Cloud Production Rate (CPR) indicates how ‘productive’ a compute or server hardware platform is. The higher the CPR, the more capacity in form of compute and storage is added. This makes it simple for a non-tech farmer to select the best farming hardware for the budget available. It is similar to the hashrate a Bitcoin miner of for example.

To calculate the CPR are very simple and straightforward formula is used:

CPR = 1.5 * the amount of Compute Units (CU) of the hardware + the amount of Storage Units (SU) of the hardware

## CPR Price:

The CPR Price is USD 40 as of Q1 2020

## Cloud Units

![](./img/cloud_units.png)

## TFTA Price

Until further notice the following USD TFTA price is used for minting: USD 0.15 plus 2% monthly starting May 2020.

## Difficulty Level

The amount of TFTA that Farmers receive for farming depends on the amount of TFT(A) that are already in circulation. The more TFT(A) already exist, the lower the rewards. This follows the principle of diminishing returns. We call this farming limitation to rewards Difficulty Level.

When the amount of existing TFT nears 4 billion, the amount of TFT received by farmers will be less. Once the maximum of 4 billion TFT has been reached, there won´t be any rewards for farming anymore.

## Calculation of TFT minted per Node per Period

> Amount of TFT = Amount of CRP * CPR Price USD / TFTA Price USD / Difficulty Level


### python pseudo farming code 

Next code is there to let you explore how the minting (farming) of tokens has been programmed in a more simple language.
This is called pseudo code which means its not the real code but should have same logic.

!!!include:farming_logic_python

### Roadmap

see [farming_minting_roadmap](farming_minting_roadmap.md)
