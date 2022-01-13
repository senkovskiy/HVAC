# HVAC
ML model to predict the Heating, ventilation, and air conditioning (HVAC) system behaviour.

This is my solution for a "Technical Session" interview at some company... 🙂

#Task Description

Attached are 4 .pkl files containing time series of exogenous influence variables, sensor data and control actions of a simulated HVAC system in form of Pandas DataFrames. Specifically, the files with the suffix "_exogenous" each contain one month of quarter-hourly timeseries relating to outdoor temperature, solar irradiance, and occupancy of the room whose temperature the HVAC system controls. The files with the suffix "_system" contain correspondingly aligned time series for the room temperature, temperatures of the water circuits of the connected boiler, temperatures of the supply air at different measuring points, a setpoint and two actuator state values as well as the delta of the gas consumption.

We now assume that today is the 31.03.2017 and the time series in the files with "train" in the name - which are from March 2017 - are known, while the time series in the file "hvac_simulation_test_exogenous.pkl" contain exact predictions of temperature, solar irradiance and occupancy of the room for April 2017.

To demonstrate your practical skills, you should now try to predict the values of the time series in the file "hvac_simulation_test_system.pkl" for all 30 days of April per day individually and as best as possible using the time series in "hvac_simulation_test_exogenous.pkl" . "Per day individually" means that in order to predict e.g. the data from "hvac_simulation_test_system.pkl" for day 3 in April, you may only use that data from "hvac_simulation_test_exogenous.pkl" as input for the model, which has a timestamp >= 2017-04-03 00:00:00 and <= 2017-04-03 23:45:00.

To train the model you can use - without restriction - all data from "hvac_simulation_train_exogenous.pkl" and "hvac_simulation_train_system.pkl".
