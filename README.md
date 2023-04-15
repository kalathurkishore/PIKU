# CVRP2D
## Overview
This repository contains the code and the data of the paper: CVRP2D: Optimized Route Navigation Considering Vehicle
Capacity for Pickup-Delivery

Submitted for the publication in SIGMOD'24. Below steps can be followed for Execution and Reproducing of the results.

## Running the Code
First unzip the `data.zip` as shown below 
```
unzip data.zip
```
Installing the required packages by 
```
pip3 install -r requirements.txt
```
Acquire Gurobi license
```
https://www.gurobi.com/downloads/free-academic-license/
```
For reproducing the results run `Markov_Approach` as shown below
```
python3 Markov_Approach.py
```
For reproducing the results run `Neural_Network_Approach` as shown below
```
python3 Neural_Network_Approach.py
```
For reproducing the results run `Decision_Focused_Learning_Approach` as shown below
```
python3 Decision_Focused_Learning_Approach.py
```
For reproducing the plots run `VRPSPD_Capacitated_plotting` accordingly based on required capacity where values were obtained from `SPD.py`

In `Figures` folder corresponding figures for the stops are provided. Here, the corresponding routes info for the respective vehicle is provided.

For `74-stops` 
```
74 stops 50000 capacity

Vehicle-1: [0, 1, 3, 5, 7, 9, 10, 11, 17, 18, 19, 20, 23, 24, 26, 28, 29, 30, 31, 34, 35, 37, 38, 40, 44, 46, 50, 53, 54, 56, 57, 58, 64, 67, 68, 72]
Vehicle-2: [0, 2, 4, 6, 8, 12, 13, 14, 15, 16, 21, 22, 25, 27, 32, 33, 36, 39, 41, 42, 43, 45, 47, 48, 49, 51, 52, 55, 59, 60, 61, 62, 63, 65, 66, 69, 70, 71, 73]

74 stops 30000 capcity

Vehicle-1: [0, 4, 6, 8, 12, 14, 15, 16, 21, 32, 33, 36, 45, 47, 48, 49, 55, 59, 60, 61, 63, 65, 66, 69, 71]
Vehicle-2: [0, 2, 3, 5, 7, 9, 10, 13, 27, 28, 30, 34, 39, 40, 41, 42, 43, 50, 51, 52, 54, 57, 58, 62, 73]
Vehicle-3: [0, 1, 11, 17, 18, 19, 20, 22, 23, 24, 25, 26, 29, 31, 35, 37, 38, 44, 46, 53, 56, 64, 67, 68, 70, 72]


74 stops 20000 capacity

Vehicle-1: [0, 3, 5, 6, 8, 9, 10, 12, 28, 40, 50, 54, 55, 57, 58, 59, 61, 65]
Vehicle-2: [0, 1, 19, 22, 30, 31, 34, 38, 44, 64]
Vehicle-3: [0, 11, 14, 17, 20, 23, 24, 25, 26, 29, 35, 36, 37, 45, 46, 56, 68, 72]
Vehicle-4: [0, 2, 7, 13, 27, 39, 41, 42, 43, 51, 52, 62, 73]
Vehicle-5: [0, 4, 15, 16, 18, 21, 32, 33, 47, 48, 49, 53, 60, 63, 66, 67, 69, 70, 71]
```
For `150-stops`
```
150 stops 50000 capacity

Vehicle-1: [0, 2, 4, 5, 12, 13, 14, 20, 23, 30, 32, 36, 37, 39, 40, 43, 44, 53, 54, 55, 59, 60, 61, 69, 72, 74, 77, 88, 91, 94, 102, 104, 107, 110, 113, 117, 125, 127, 130, 134, 141, 145]
Vehicle-2: [0, 8, 25, 27, 34, 45, 46, 58, 63, 67, 75, 78, 83, 84, 90, 93, 100, 111, 119, 121, 126, 137, 138, 139, 140, 142, 147, 148]
Vehicle-3: [0, 1, 7, 9, 10, 11, 15, 17, 18, 19, 38, 41, 49, 52, 62, 65, 73, 80, 82, 85, 87, 97, 98, 101, 103, 105, 108, 109, 112, 114, 116, 118, 120, 122, 128, 129, 131, 133]
Vehicle-4: [0, 3, 6, 16, 21, 22, 24, 26, 28, 29, 31, 33, 35, 42, 47, 48, 50, 51, 56, 57, 64, 66, 68, 70, 71, 76, 79, 81, 86, 89, 92, 95, 96, 99, 106, 115, 123, 124, 132, 135, 136, 143, 144, 146, 149]

150 stops 30000 capacity

Vehicle-1: [0, 2, 5, 7, 18, 20, 23, 36, 39, 52, 54, 60, 74, 85, 88, 98, 101, 102, 105, 108, 120, 122, 134, 141]
Vehicle-2: [0, 9, 10, 11, 29, 31, 49, 62, 70, 79, 82, 106, 115, 123, 129, 131, 132, 133, 136, 146]
Vehicle-3: [0, 21, 22, 28, 30, 32, 33, 43, 44, 51, 53, 55, 64, 66, 72, 73, 76, 89, 91, 96, 104, 107, 113, 117, 124, 125, 127, 130, 143, 145, 149]
Vehicle-4: [0, 8, 25, 27, 34, 45, 46, 58, 63, 67, 75, 78, 83, 84, 90, 93, 100, 111, 119, 121, 126, 137, 138, 139, 140, 142, 147, 148]
Vehicle-5: [0, 1, 4, 6, 12, 13, 14, 15, 17, 37, 38, 40, 41, 48, 59, 61, 65, 69, 77, 80, 87, 94, 95, 103, 110, 112, 114]
Vehicle-6: [0, 3, 16, 19, 24, 26, 35, 42, 47, 50, 56, 57, 68, 71, 81, 86, 92, 97, 99, 109, 116, 118, 128, 135, 144]

150 stops 20000 capacity

Vehicle-1: [0, 1, 6, 21, 48, 66, 73, 76, 82, 89, 95, 96, 115, 124, 132, 149]
Vehicle-2: [0, 2, 5, 27, 36, 54, 60, 63, 74, 75, 83, 98, 102, 105, 119, 120, 126, 134, 139]
Vehicle-3: [0, 10, 11, 29, 31, 33, 41, 51, 70, 79, 106, 123, 131, 133, 136, 146]
Vehicle-4: [0, 7, 18, 20, 23, 39, 52, 65, 85, 88, 101, 103, 108, 114, 122, 141]
Vehicle-5: [0, 8, 25, 45, 46, 58, 67, 78, 84, 90, 93, 100, 111, 121, 137, 138, 140, 142, 147, 148]
Vehicle-6: [0, 4, 12, 13, 14, 15, 17, 32, 37, 38, 40, 43, 59, 61, 69, 77, 80, 87, 94, 107, 112]
Vehicle-7: [0, 9, 19, 49, 62, 97, 109, 116, 118, 128]
Vehicle-8: [0, 3, 16, 24, 26, 35, 42, 47, 50, 56, 57, 68, 71, 81, 86, 92, 99, 129, 135, 144]
Vehicle-9: [0, 22, 28, 30, 34, 44, 53, 55, 64, 72, 91, 104, 110, 113, 117, 125, 127, 130, 143, 145]
```
For `200 stops`
```
200 stops 50000 capacity

Vehicle-1: [0, 9, 12, 18, 22, 25, 30, 37, 39, 48, 58, 64, 77, 79, 80, 89, 96, 98, 101, 106, 107, 108, 109, 110, 126, 149, 150, 152, 153, 155, 157, 158, 169, 175, 176, 181, 182, 184, 185, 186, 190, 193, 195, 197]
Vehicle-2: [0, 3, 8, 11, 13, 15, 17, 23, 26, 31, 38, 53, 59, 62, 66, 71, 76, 78, 82, 83, 86, 90, 93, 94, 104, 118, 122, 137, 145, 164, 168, 178, 183, 189, 192]
Vehicle-3: [0, 14, 29, 34, 44, 46, 47, 51, 56, 72, 87, 95, 100, 105, 111, 113, 114, 120, 125, 128, 132, 141, 143, 163, 165, 167, 177, 194]
Vehicle-4: [0, 19, 21, 24, 27, 33, 43, 49, 50, 52, 54, 55, 57, 60, 63, 67, 68, 69, 70, 73, 74, 75, 81, 84, 88, 99, 102, 103, 112, 115, 116, 117, 119, 121, 124, 127, 130, 133, 134, 135, 138, 148, 154, 160, 161, 162, 166, 170, 180, 187, 196, 198, 199]
Vehicle-5: [0, 1, 2, 4, 5, 6, 7, 10, 16, 20, 28, 32, 35, 36, 40, 41, 42, 45, 61, 65, 85, 91, 92, 97, 123, 129, 131, 136, 139, 140, 142, 144, 146, 147, 151, 156, 159, 171, 172, 173, 174, 179, 188, 191]

200 stops 30000 capacity

Vehicle-1: [0, 5, 6, 20, 25, 30, 32, 42, 45, 64, 85, 89, 97, 101, 102, 126, 131, 144, 146, 153, 176, 181, 185, 186, 188, 191]
Vehicle-2: [0, 12, 22, 28, 35, 39, 41, 58, 77, 79, 80, 92, 98, 108, 110, 142, 150, 152, 157, 158, 169, 174, 175, 184, 190, 193]
Vehicle-3: [0, 24, 27, 33, 50, 57, 60, 63, 68, 69, 73, 81, 84, 88, 103, 112, 115, 116, 121, 124, 127, 134, 160, 161, 170, 196, 199]
Vehicle-4: [0, 14, 16, 21, 29, 34, 37, 44, 47, 55, 67, 87, 105, 113, 114, 117, 132, 135, 138, 141, 143, 155, 163, 165, 167, 171, 177, 194, 198]
Vehicle-5: [0, 19, 43, 46, 49, 51, 52, 54, 56, 70, 72, 74, 75, 95, 99, 100, 111, 119, 120, 125, 128, 130, 133, 148, 162, 166, 180]
Vehicle-6: [0, 2, 4, 7, 10, 23, 36, 48, 59, 61, 62, 65, 71, 78, 90, 91, 93, 104, 136, 139, 147, 151, 159, 164, 173, 192]
Vehicle-7: [0, 3, 8, 11, 13, 31, 76, 83, 118, 137, 154, 178, 187]
Vehicle-8: [0, 1, 9, 15, 17, 18, 26, 38, 40, 53, 66, 82, 86, 94, 96, 106, 107, 109, 122, 123, 129, 140, 145, 149, 156, 168, 172, 179, 182, 183, 189, 195, 197]

200 stops 20000 capacity

Vehicle-1: [0, 15, 40, 66, 86, 96, 107, 122, 156, 183]
Vehicle-2: [0, 6, 12, 16, 22, 35, 41, 50, 57, 80, 98, 108, 116, 127, 152, 157, 174, 175]
Vehicle-3: [0, 5, 25, 58, 61, 64, 79, 89, 101, 126, 144, 153, 173, 176, 185]
Vehicle-4: [0, 43, 49, 52, 70, 74, 75, 166]
Vehicle-5: [0, 7, 17, 23, 36, 38, 59, 62, 65, 71, 78, 82, 90, 93, 94, 104, 145, 164, 168, 189, 192]
Vehicle-6: [0, 14, 29, 34, 37, 44, 47, 87, 105, 113, 132, 141, 155, 163, 165, 167, 177, 194]
Vehicle-7: [0, 19, 51, 54, 56, 95, 99, 100, 111, 119, 120, 125, 128, 130, 133, 148, 162, 180]
Vehicle-8: [0, 33, 46, 55, 63, 69, 72, 73, 88, 114, 115, 117, 134, 138, 143, 161, 170, 198]
Vehicle-9: [0, 2, 4, 10, 26, 30, 48, 53, 91, 136, 139, 147, 151, 159]
Vehicle-10: [0, 3, 8, 11, 13, 31, 76, 83, 118, 137, 154, 178, 187]
Vehicle-11: [0, 1, 20, 28, 32, 42, 85, 97, 123, 129, 131, 146, 149, 171, 181, 182, 186, 191]
Vehicle-12: [0, 9, 18, 39, 45, 92, 106, 109, 140, 142, 150, 169, 172, 179, 184, 188, 190, 195, 197]
Vehicle-13: [0, 21, 24, 27, 60, 67, 68, 77, 81, 84, 102, 103, 110, 112, 121, 124, 135, 158, 160, 193, 196, 199]
```
