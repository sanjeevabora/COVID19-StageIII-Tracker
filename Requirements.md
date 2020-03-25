# COVID19
COVID19 Technology Platform 
 Introduction: The idea is to build an app where we collect data from the individuals regarding their symptoms, travel history and use this data to sort them into different risk categories (Red, Orange, Yellow and Green). This data will be used to caution users and provide information regarding areas that are high risk and to calculate the number of touch points they have.  

Phase 1: COVID19 Stage III Tracker App 
Planned Release by 1st April,2020 for Android
Release Targets:
1.	Sign Up
2.	Profile Setup with 
a.	General Information
b.	Existing Health History
c.	Symptoms
d.	Travel History and Exposure
i.	Includes manual entries as well as data from Google Maps
3.	Determine Risk Factor and Alert Users
a.	Provide advice on next steps in case of exposure
b.	Alert users if a high risk individual is in the vicinity
c.	Create Risk zones (High/ Medium/ Low) based on the data
4.	Provide a cloud solution for local authorities to monitor the situation using Heat Maps
Detailed Requirements: 
 
I.	Sign Up using 2-step Verification 
The user will download the app from the store and sign-up with their mobile number using a 2-step verification process 
 
II.	Profile Setup 
The following data is collected from the user to determine their exposure and risk 
a.	General Information: Name, Age, Gender, Area of Residence 
b.	Existing Health History: This is to determine if the user is at a higher risk  
c.	Symptoms  
i.	Level 1: Temperature, Cough, Cold, Body Aches, Sore Throat, Headache 
ii.	Level 2: Moderate to Severe Cough, Breathlessness, Difficulty in Breathing, Persistent Pain, Severe Weakness 
An existing API or application can be used to calculate the severity of the symptoms. An Alternative would be to build a point based calculator 
 
d.	Travel History and Exposure 
The user will be asked to provide their travel history for the past 14 days. The following data will be collected and it will be used to determine the exposure they had to the COVID-19 virus and the probability that they could be carriers is calculated 
i.	Out of Country Travel  
ii.	Interstate/ City Travel  
iii.	Within the City Travel – Public areas like Markets, Super Markets, Airports, Railway Stations etc. Are areas with high exposure 
iv.	Contact with individuals with confirmed COVID in the past 14 days 
A point system will be used to determine the exposure levels 
 
III.	Determine Risk Factor and Alert Users 
A combination of Health History, Symptoms and Travel History is used to determine the risk factor and categorize the user into different zones. This data will be used for the following, 
a.	Provide advice to users according to their risk factor and local health care contact details if required.  
For example: User with high exposure and mild to no symptoms will be advised to self-isolate. Additional info regarding self-isolation will be provided 
•	As much as possible, you should limit your contact with people other than the family members/companions you travelled with 
•	You should avoid having visitors to your home 
•	But it is okay for friends, family or delivery drivers to drop off food and supplies 
b.	Alert other users if a high risk individual is in their immediate area 
c.	Continuous Background sensing and Touch Point calculation 
i.	Determine regions/zones and represent them using color codes  
ii.	User will be able to search for an area and see if it is a high risk zone 
iii.	Alert and warn the user based on touchpoints and the profile of the touchpoints 
iv.	Advise the user on next steps (wash hands/ Self-isolation/ see doctor) based on the exposure (See III. a) 
 
IV.	Ability to trace and identify potential threats based on their profile and travel history 
Using Google Maps, the users travel history can be mapped for the past 14 days and this data can be used to identify potential threats and 
a.	Alert users with valid info 
b.	Share with local authorities about threats and zones. A cloud login can be provided for local authorities to access this information 
V.	 Cloud design & architecture 
a.	Privacy first architecture  
The privacy of the user is paramount. User information is not shared with anyone except with the local authorities in case of positive cases 
b.	User, Role and permissions management 
c.	Loosely coupled architecture for extensibility  
d.	Local authorities interface to monitor Stage III users and their vulnerabilities (Best UX with heat chart for easy tracing for authorities) 
5. Integration with other open APIs for travel, disease, alert related data.  

 

