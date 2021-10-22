# Phase-detection

This paper provides a data-driven method for traffic phase and detector type detection in signalized intersections using high-resolution event-based data. Event data stores the timestamps associated with a detector on and detector off related to detector occupancy and vehicle actuation. Moreover, it keeps the timestamp of a signal event (for instance, phase on, phase green termination, etc.). The data preparation starts by filtering data to different data tables and connecting them through each cycle's start and end times. Later we aggregate the data into multiple five seconds time chunks and propose a machine learning method, occupancy Pattern Association (OPA), to identify the detector type and associated phase. Automated traffic signal performance measures (ATSPM) enable traffic control and operation in an efficient manner. The high-resolution data capability can be used to generate performance measures allowing practitioners to track signal operations. Traffic volume in each phase and the detection type is a requirement for most performance measures. There is a lack of reliable, standard meta-data to do broader analysis across different corridors and agencies. This framework addresses that challenge by providing a machine learning-based method for phase movement detection and detector type identification.
![Alt text](phase.png?raw=true "Title")

In this study, we used high-resolution event data for Dodge Street corridors of Omaha in Nebraska and Foothill drive and 20th highway in Utah. There are 9 intersections along Dodge street corridor and 9 intersections in Foothill drive street. We used five and four day’s data for Highway 20th street and foothill corridors in Utah, and six days’ data for Dodge street corridors in Omaha, Nebraska. (Bellow) shows the location of these three corridors in our analysis.
![Alt text](dodge.png?raw=true "Title")
![Alt text](foothil.png?raw=true "Title")
![Alt text](20.png?raw=true "Title")
