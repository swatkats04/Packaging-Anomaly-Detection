# Packaging-Anomaly-Detection

The aims of this experiment were to detect the anomalies resulting from the stretching of the chain.

## Dataset 

This dataset has been collected during an experiment on a packaging production line. The chain of the production line has been monitored on a normal mode on the first part of the dataset.

Then, the chain has been stretched out while the production kept being monitored. The data were aggregated at the minutes using the median.

The column flag is used to distinguished the two periods. It equals 1 when the chain of the production line is tensed and 0 when the chain is loose.

### Column Description 

timeindex- Number of seconds since the beginning of the experiment\
flag- Indicates the normal period (1) and the suspected anomalous period (0)\
currentBack-Current of the rear motor\
motorTempBack-TemperapositionBack\
positionBack- Position of the rear chain\
refPositionBack- Reference position of the rear chain\
refVelocityBack- Reference velocity of the rear chain\
trackingDeviationBack-Tracking deviation of the rear chain\
velocityBack-Velocity of the rear chain\
currentFront- Current of the front motor\
motorTempFront- Temperature of the front motor\
positionFront- Position of the front chain\
refPositionFront-Reference position of the front chain\
refVelocityFront- Reference velocity of the front chain\
trackingDeviationFront - Tracking deviation of the front chain\
velocityFront - Velocity of the front chain

## Result 
Random Forest gave the highest F1-score of approx. 85%, and hence this model was used to predict the class labels for the test dataset.

#### Acknowledgements
Schneider Electric Exchange for providing this dataset.
