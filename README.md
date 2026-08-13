A PROJECT TITLE 
ON 
Accident Hotspot Detection Using DBSCAN-Based Anomaly Detection 
project report submitted in partial fulfilment of the requirements for the Course 
MACHINE LEARNING 
BACHELOR OF TECHNOLOGY 
in 
A.Y.: 2026-27 
by 
Bathula Neha 
Veeramallu Rohita Sai Lakshmi 
Koumudi 
Roll No: 2520090013 
Roll No: 2520090235 
Roll No: 2520090161 
Under the Esteemed guidance of 
Haritha 
Assistant Professor, Department of CS&IT 
DEPARTMENT OF CS&IT 
Accident Hotspot Detection Using DBSCAN-Based Anomaly Detection 
1. Abstract: 
Road accidents remain a serious concern across urban and rural areas, resulting in loss of life, injuries, 
and significant property damage, often occurring repeatedly at specific locations due to poor road 
conditions, congestion, sharp turns, inadequate lighting, or traffic-rule violations. Identifying such 
accident-prone locations manually is difficult, time-consuming, and prone to oversight. This project 
presents a Machine Learning-based Accident Hotspot Detection System that applies DBSCAN 
(Density-Based Spatial Clustering of Applications with Noise), an unsupervised clustering algorithm, 
to automatically discover accident hotspots from historical accident records while treating isolated 
incidents as anomalies. Unlike traditional clustering techniques, DBSCAN does not require the number 
of clusters to be specified in advance, can detect irregularly shaped clusters, and handles noisy 
geospatial data effectively, making it well suited for location-based accident analysis. The dataset is 
drawn from publicly available sources such as the US Accidents Dataset, UK Road Safety Dataset, or 
Indian Road Accident Dataset, and includes features such as accident latitude and longitude, date, time, 
road type, speed limit, weather conditions, visibility, road surface condition, junction type, traffic signal 
presence, accident severity, and number of vehicles involved. The workflow involves data collection, 
preprocessing, exploratory data analysis, feature selection of key spatial and contextual attributes, and 
application of the DBSCAN algorithm using tuned eps and min_samples parameters to group nearby 
accident locations into clusters. Clustering quality is assessed using the Silhouette Score, Davies
Bouldin Index, visual inspection, and domain expert validation. The resulting system classifies 
locations as high-risk hotspots, medium-risk areas, low-risk areas, or isolated anomalies, and visualizes 
results on interactive maps using tools such as Folium and Plotly. This project supports applications 
including smart city traffic management, road safety analysis, accident prevention planning, emergency 
response optimization, and insurance risk assessment. Future enhancements include integrating real
time accident reporting, combining live GPS, weather, and traffic data for dynamic hotspot detection, 
developing an interactive web or mobile application, applying deep learning for severity prediction, and 
recommending safer alternative routes based on detected hotspots. 
2. INTRODUCTION: 
Road traffic accidents continue to pose a major public safety challenge, often clustering around specific 
locations due to factors such as poor road design, heavy congestion, sharp turns, inadequate lighting, or 
frequent traffic-rule violations. Traditional approaches to identifying these accident-prone locations rely 
heavily on manual analysis of accident reports, which is slow, inconsistent, and difficult to scale across 
large regions. With the growing availability of geo-tagged accident records from government portals 
and open datasets, unsupervised machine learning techniques can be applied to automatically detect 
spatial patterns in accident occurrence. This project uses DBSCAN, a density-based clustering 
algorithm well suited to spatial data, to group accident locations into meaningful hotspot clusters while 
identifying isolated incidents as anomalies. Unlike centroid-based clustering methods, DBSCAN does 
not require the number of clusters to be predefined and can detect irregularly shaped, dense regions, 
making it particularly effective for real-world accident data. The resulting hotspot map is intended to 
support traffic authorities, urban planners, and emergency services in prioritizing road safety 
interventions and allocating resources more effectively. 
3. SOFTWARE REQUIREMENTS: 
Programming Language: Python 3.x 
Libraries: Pandas, NumPy, Scikit-learn (DBSCAN), Matplotlib, Seaborn, Folium, Plotly 
Development Environment: Jupyter Notebook / Google Colab / Visual Studio Code 
Operating System: Windows / Linux / macOS 
Signature of the Guide 
Course Instructor
