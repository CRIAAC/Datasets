This work was achieved by Ph.D. students affiliated to the LIARA Laboratory at the Uniersité du Québec à Chicoutimi.

http://liara.uqac.ca/

Version
-------
1.0

Datasets
--------
1/ soil_types
2/ soil_types_participant
3/ soil_types_position

Independencies
--------------
Seperated datasets for both user and position in order to verify if data are either or both, user-independant or position-independent. 

	- 1 dataset per position: backpack, left_pocket, left_hand_bag, right_hand_bag, right_pocket.
	- 1 dataset per participant: A, B, C, D, E, F, G, H, I.


Attributes
----------
For each dataset, attributes refers to both time and frequency domain features, being 70 features in total. To convert the original signal from time domain to its representation in frequency domain, we have used the Fast Fourier Transform (FFT) algorithm.

	- Time domain: Mean for each axis and on all axis; Standard deviation for each axis and on all axis; Skewness for each axis and on all axis; Kurtosis for each axis and on all axis; Zero-Crossing-Rate for each axis and on all axis; Correlation between for all possible axis combinations.

	- Frequency domain: DC Component for each axis; Energy for each axis; Entropy for each axis.

Classes
-------

	1/ soil types in {cement, gravel, snow, sand}.
	2/ soil types for each given participant in {cement_A, cement_B,..., sand_I}.
	3/ soil types for each given position in {cement_backpack, cement_left_pocket,..., sand_right_pocket}.

Authors
-------
	- Valère Plantevin, LIARA Laboratory, Université du Québec à Chicoutimi, QC, Canada.
			--> valere.plantevin1@uqac.ca
	- Florentin Thullier, LIARA Laboratory, Université du Québec à Chicoutimi, QC, Canada.
			--> florentin.thullier1@uqac.ca

Licence
-------
Copyright 2017 LIARA Laboratory.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

