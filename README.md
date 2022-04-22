# Heart Attack Survival
Predict if a patient will survive for at least one year following a heart attack, using UCI Echocardiogram Data Set[[1]](#1). (This is only for educational purpose)

## Dataset

- **Data Set Characteristics**: Multivariate.
- **Associated Tasks**: Classification.

### Attributes
1. **survival**: the number of months patient survived (has survived, if patient is still alive). Because all the patients had their heart attacks at different times, it is possible that some patients have survived less than one year but they are still alive. Check the second variable to confirm this. Such patients cannot be used for the prediction task mentioned above.
2. **still-alive**: a binary variable. 0=dead at end of survival period, 1 means still alive.
3. **age-at-heart-attack**: age in years when heart attack occurred.
4. **pericardial-effusion**: binary. Pericardial effusion is fluid around the heart. 0=no fluid, 1=fluid.
5. **fractional-shortening**: a measure of contracility around the heart lower numbers are increasingly abnormal.
6. **epss**: E-point septal separation, another measure of contractility. Larger numbers are increasingly abnormal.
7. **lvdd**: left ventricular end-diastolic dimension. This is a measure of the size of the heart at end-diastole. Large hearts tend to be sick hearts.
8. **wall-motion-score**: a measure of how the segments of the left ventricle are moving.
9. **wall-motion-index**: equals wall-motion-score divided by number of segments seen. Usually 12-13 segments are seen in an echocardiogram. Use this variable INSTEAD of the wall motion score.
10. **mult**: a derivate var which can be ignored.
11. **name**: the name of the patient (I have replaced them with "name")
12. **group**: meaningless, ignore it.
13. **alive-at-1**: Boolean-valued. Derived from the first two attributes. 0 means patient was either dead after 1 year or had been followed for less than 1 year. 1 means patient was alive at 1 year.

## Before we start
Run the file PreparingDataSet.ipynb in Goggle Colab to remove null and unnecessary values from the data set.


## References

<a id="1">[1]</a> 
Dua, D. and Graff, C. (2019). [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml). Irvine, CA: University of California, School of Information and Computer Science.
