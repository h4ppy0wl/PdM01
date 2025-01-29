In this project I am going to explore different Failure Analysis techniques in various industrial applications.
The project is ongoing, so more datasets and more analysis will be added to the project. I will keep the project organized by using dedicated folders for each dataset.

I follow CRISP-DM methodology in my analysis following these steps:

1. Business Understanding:
Defining business objectives
Assessing the current situation
Determining data mining goals
Producing a project plan

2. Data Understanding:   
Gathering initial data
Describing data
Exploring data
Verifying data quality

3. Data Preparation:
Selecting data
Cleaning data
Constructing data (feature engineering)
Integrating data
Formatting data

4. Modeling:
Selecting modeling techniques
Designing tests
Building the model
Assessing the model

5. Evaluation:
Evaluating results
Reviewing the process
Determining the next steps

6. Deployment:
Planning deployment
Monitoring and maintenance
Reviewing the project
Finalizing the project


**Bearing Fault Detection 01**

DE - drive end accelerometer data
FE - fan end accelerometer data
IR - Inner Race
OR - Outer Race
NB - Normal Baseline
Fault Diameters: 0.007" and 0.021"

-> OR-21 = 0.021" fault on outer diameter

Drive End (DE) Accelerometer: Near the motor drive end.
Fan End (FE) Accelerometer: Near the opposite end (fan side).
The presence of both DE and FE accelerometer data helps in analyzing how bearing faults propagate along the shaft and how their signatures differ at different positions.

Each accelerometer captures different aspects of fault propagation:

(A) Drive End (DE) Accelerometer
Directly affected by shaft forces and misalignment.
Captures stronger vibration signals from inner race, ball, and drive-end outer race faults.
Fault signals do not get dampened as much since they are closer to the source.

(B) Fan End (FE) Accelerometer
Located further from the main load and drive forces.
Captures weaker but more global vibration signals.
Outer race faults on the fan-end bearing may be easier to detect here.
Some shaft-related issues (misalignment, unbalance) may be more pronounced here.

Benefits of Having Both Sensors
1️⃣ Identifying Fault Location
If a fault is stronger in DE data, it is likely at the drive-end bearing.
If a fault is stronger in FE data, it is likely at the fan-end bearing.
2️⃣ Understanding Fault Propagation
Vibration signals travel through the shaft differently.
Having both datasets allows engineers to study how faults spread from one end of the system to another.
3️⃣ Differentiating Between Local & Global Vibrations
DE detects more localized effects from faults near the motor load.
FE detects overall system vibrations, including shaft misalignment or resonance.
4️⃣ Reducing Misdiagnosis
If only one sensor were used, some faults could be missed or misinterpreted.
For example, a shaft misalignment issue may be subtle on the DE but stronger on the FE.