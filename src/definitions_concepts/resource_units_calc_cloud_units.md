
Transformation between resource units (CRU, MRU, HRU, SRU) and cloud units (CU, SU); basically how does the software translate measured capacity to capacity which gets sold/bought.

1 SU is 1 TB of HD capacity and 40 GB of SSD capacity with a buffer of 20%

```python
su = (hru / 1000 + sru / 100 / 2) / 1.2
```


Basically 1 CU is 2 virtual CPU with max oversubscription on CPU core of 4 and min required memory is 4GB. Oversubscription of 4 is still gentle we know that many other providers use more.

```python
cu = min((mru - 1) / 4, cru * 2)	 
```

We substract 1 GB of memory for the operating system to function.



