# Phase-detection

This paper provides a data-driven method for traffic phase and detector type detection in signalized intersections using high-resolution event-based data. Event data stores the timestamps associated with a detector on and detector off related to detector occupancy and vehicle actuation. Moreover, it keeps the timestamp of a signal event (for instance, phase on, phase green termination, etc.). The data preparation starts by filtering data to different data tables and connecting them through each cycle's start and end times. Later we aggregate the data into multiple five seconds time chunks and propose a machine learning method, occupancy Pattern Association (OPA), to identify the detector type and associated phase. Automated traffic signal performance measures (ATSPM) enable traffic control and operation in an efficient manner. The high-resolution data capability can be used to generate performance measures allowing practitioners to track signal operations. Traffic volume in each phase and the detection type is a requirement for most performance measures. There is a lack of reliable, standard meta-data to do broader analysis across different corridors and agencies. This framework addresses that challenge by providing a machine learning-based method for phase movement detection and detector type identification.

<p align="center">
  <img src="phase.png" width="500"/>
</p>




In this study, we used high-resolution event data for Dodge Street corridors of Omaha in Nebraska and Foothill drive and 20th highway in Utah. There are 9 intersections along Dodge street corridor and 9 intersections in Foothill drive street. We used five and four day’s data for Highway 20th street and foothill corridors in Utah, and six days’ data for Dodge street corridors in Omaha, Nebraska. (Bellow) shows the location of these three corridors in our analysis.
<p align="center">
  <img src="dodge.png.jpg" width="500"/>
  <img src="foothil.png" width="500"/>
  <img src="20.png.jpg" width="500"/>
</p>



Performance 

|    Foothill drive          |                        |                 | Dodge street               |                        |                 | Highway 20                 |                         |                 |
|----------------------------|------------------------|-----------------|----------------------------|------------------------|-----------------|----------------------------|-------------------------|-----------------|
|     Number of detectors    |     Intersection id    |     Accuracy    |     Number of detectors    |     Intersection id    |     Accuracy    |     Number of detectors    |     Intersection id     |     Accuracy    |
|     24                     |     7216               |     1           |     20                     |     85                 |     1.00        |     16                     |     Century             |     0.87        |
|     19                     |     7217               |     0.79        |     44                     |     86                 |     0.89        |     14                     |     Crescent Ridge      |     0.86        |
|     16                     |     7218               |     0.87        |     25                     |     90                 |     0.85        |     17                     |     Devon               |     0.59        |
|     25                     |     7219               |     0.84        |     30                     |     91                 |     0.97        |     14                     |     JFK                 |     0.79        |
|     17                     |     7220               |     0.94        |     25                     |     92                 |     0.85        |     19                     |     NW Arterial         |     0.79        |
|     5                      |     7221               |     1.00        |     26                     |     93                 |     0.8         |     15                     |           University    |     0.73        |
|     2                      |     7223               |     0.50        |     14                     |     94                 |     1.00        |     8                      |     Wacker              |     0.75        |
|     9                      |     7371               |     0.67        |     36                     |     95                 |     0.69        |     -                      |     -                   |     -           |
|     2                      |     7503               |     1.00        |     12                     |     102                |     1.00        |     -                      |     -                   |     -           |
