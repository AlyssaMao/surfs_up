# surfs_up

## Overview of Project

### Purpose
The purpose of this analysis is to inform W. Avy as to whether Oahu is an ideal location to open a surf shop based on temperature and precipitation. 

## Results

3 major points from the two analysis performed during the challenge is as follows:

1. June had a mean temperature of 74.9 whereas December had a mean temperature of 71, which makes sense because June is summer time and December is winter time, thus June has the higher average temperature. 

2. June had a count of 1700 temperatures whereas December only had a count of 1517 temperatures

3. December had a standard deviation of 3.745 while June had a standard deviation of 3.257, signifying that December had a larger spread of different temperatures. 
  
### Summary

**How many roles will need to be filled as the "silver tsunami" begins to make an impact?**

Referencing the images cited above in the results section, a total of 29414 Senior Engineers, 28254 Senior Staff, 14222 Engineers, 12243 Staff, 4502 Technique Leader, 1761 Assistant Engineer, and 2 Managers will be retiring and these roles will need to be filled by a wave of next generation new hires. 

**Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?**

Two additional queries we can perform to gather more weather data for June and December would be the following:

1. Look at the precipitation amount for June by refactoring our code from the challenge to look like this 

```
results = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date) == 6).all()
```
2. Look at the precipitation amount for December by refactoring our code from the challenge to look like this

```
results = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date) == 12).all()
```

