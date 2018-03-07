# SoilTypesRecognition Dataset

[![Licence Apache2](https://img.shields.io/hexpm/l/plug.svg)](http://www.apache.org/licenses/LICENSE-2.0)

---

Datasets
---
* __soil_types__
* __soil_types_participant__
* __soil_types_position__

Attributes
---
* For each dataset under the __raw__ folder, attributes refers to raw data produced by each axis of the IMU in __[acc_x, acc_y, acc_z, gyr_x, gyr_y, gyr_z, mag_x, mag_y, mag_z]__.
* For each dataset under the __feature__ folder, attributes refers to both time and frequency domain features. To convert the original signal from time domain to its representation in frequency domain, we have used the Fast Fourier Transform (FFT) algorithm.

	* Time domain: Mean for each axis and on all axis; Standard deviation for each axis and on all axis; Skewness for each axis and on all axis; Kurtosis for each axis and on all axis; Zero-Crossing-Rate for each axis and on all axis; Correlation between for all possible axis combinations.

	* Frequency domain: DC Component for each axis; Energy for each axis; Entropy for each axis.

Classes
---
1. soil types in __[cement, gravel, snow, sand]__.
2. soil types for each given participant in __[cement_A, cement_B,..., sand_I]__.
3. soil types for each given position in __[cement_backpack, cement_left_pocket,..., sand_right_pocket]__.

Independencies
---
Seperated datasets are provided for both user and position in order to verify if data are either or both, user-independant or position-independent. 

* One dataset per position in __[backpack, left_pocket, left_hand_bag, right_hand_bag, right_pocket]__.
* One dataset per participant in __[A, B, C, D, E, F, G, H, I]__.

Authors
---
This work was achieved by Ph.D. students affiliated to the **[LIARA laboratory](http://liara.uqac.ca/)** at the Uniersité du Québec à Chicoutimi.

* __[Florentin Thullier](florentin.thullier1@uqac.ca)__, LIARA Laboratory, Université du Québec à Chicoutimi, QC, Canada.
* __[Valère Plantevin](valere.plantevin1@uqac.ca)__, LIARA Laboratory, Université du Québec à Chicoutimi, QC, Canada.

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

