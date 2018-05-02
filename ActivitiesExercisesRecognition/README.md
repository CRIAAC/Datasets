# ActivitiesExercisesRecognition Dataset

[![Licence Apache2](https://img.shields.io/hexpm/l/plug.svg)](http://www.apache.org/licenses/LICENSE-2.0)

---

Raw data
---

* For each dataset under the **raw** folder, attributes refer to raw data produced by each axis of the IMU. A LSM9DS1 has been used, revealing data from an accelerometer **[ax, ay, az]**, a gyroscope **[gx, gy, gz]** and a magnetometer **[mx, my, mz]** .
* The following table indicates each exercice or activity, the way data it has been recorded, and a short description.  

| Exercice/Activity         | Recording                 | Description                           |    
| -------------             |:-------------:            |:-----:                                |
| ExoFente                  | Iteration per iteration   | Typical Front Lunge                   |
| ExoMarche                 | Iteration per iteration   | Front Step Down                       |    
| ExoSitUp                  | Iteration per iteration   | Sit-to-Stand                          |
| ExoSquat                  | Iteration per iteration   | Typical Squat on chair                |
| shortRunning              | Continued                 | Continuously running for 30 seconds   |
| shortSeat                 | Continued                 | Staying sit in a chair for 30 seconds |
| shortSitting              | Iteration per iteration   | Transition Stand-to-Sit               |
| shortStanding             | Iteration per iteration   | Transition Sit-to-Stand               |
| shortSwitch               | Iteration per iteration   | Fast rotation of the wrist            |
| shortWalking              | Continued                 | Continuously walking for 30 seconds   |

* Features can be extracted from these raw data, to perform activity recognition with data mining algorithm. An example of features extraction can be found in the **features** folder, and an article using this dataset can be read in this article :


    Chapron, K.; Plantevin, V.; Thullier, F. A More Efficient Transportable and Scalable System for Real-Time Activities and Exercises Recognition. Sensors 2018, 18, 268, doi:10.3390/s18010268. 

Features extracted from raw data
---

Every features extracted have been combined in a single file available in the **features** folder. Lines can be described as followed : 

    val_feature1, val_feature2, ..., val_feature104, val_feature105, CLASS, PARTICIPANT

The features are listed in the following list : 
* **TEMPORAL DOMAIN**
    * (9) **Mean value** for each axis of every device
    * (3) **Mean value of mean values** for each device
    * (9) **Standard Deviation** for each axis of every device
    * (3) **Mean value of standard deviation** for each device
    * (9) **Skewness Value** for each axis of every device
    * (3) **Mean value of Skewness value** for each device
    * (9) **Kurtosis Value** for each axis of every device
    * (3) **Mean value of Kurtosis value** for each device
    * (9) **Zero Crossing Rate** for each axis of every device
    * (3) **Mean value of Zero Crossing Rate** for each device
    * (18) **Correlation** between every axis of every device
* **FREQUENTIAL DOMAIN**
    * (9) **DC Component** for each axis of every device
    * (9) **Energy** for each axis of every device
    * (9) **Entropy** for each axis of every device
* **TOTAL**
    * It results in **105** features.
  
The classes can be observed in the table in the precedent chapter.  
The participants are represented by the letters A to J.


Authors
---
This work was achieved by Ph.D. students affiliated to the **[LIARA laboratory](http://liara.uqac.ca/)** at the Uniersité du Québec à Chicoutimi.

* __[Kévin Chapron](kevin.chapron1@uqac.ca)__, LIARA Laboratory, Université du Québec à Chicoutimi, QC, Canada.
* __[Valère Plantevin](valere.plantevin1@uqac.ca)__, LIARA Laboratory, Université du Québec à Chicoutimi, QC, Canada.
* __[Florentin Thullier](florentin.thullier1@uqac.ca)__, LIARA Laboratory, Université du Québec à Chicoutimi, QC, Canada.

Licence
---
Copyright 2018 LIARA Laboratory.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.