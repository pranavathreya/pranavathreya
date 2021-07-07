# The Beauty of the Big Data Platform
A well-engineered Big Data Platform is truly a sight to behold. It's hard to list all of the aspects that fuel my love for these systems, but the most apparent would be the fascinating design solutions that allow the platform to scale rapidly, provide the lowest latency to its customers, onboard new technologies with ease and do many more amazing things.

This github profile is a means for me to document and catalog my passion for these platforms and the design principles I've learnt that go into making them 'scalable, reliable and easy-to-use'. 

## Inferences from the Evolution of Uber's Big Data Platform
*This is a work in progress that I add to as I read through this blog multiple times: https://eng.uber.com/uber-big-data-platform/*

### With any Big Data Platform, Prioritize the Following
- reliability (Low-latency, always-online)
- scalability
- ease-of-use
	
### Gen 1
* Features:
  * data resided in multiple OLTP databases (inserting, updating or deleting small amounts of data)
  * engineers had to access databases individually and write their own code to combine it
  * no global access to ALL the data
  * total data size: a few TBs
  * latency: often sub-minute; 'very fast'; apparently because each database was queried directly as well as the data being stored in an online transactional DB.
		

### Lessons Learnt
- Formal contract between data producers and consumers in order to make ETL pipelines robust to change.
- Standardization of ingestion jobs allows for ease in adding new datasets and types.
- Horizontal scalability is critical in shortening the time to onboard ad-hoc services, thus allowing time to work on building the next generation of the data platform.
- Hadoop Data Lake:
	- All raw data ingested data from different online data stores ONLY ONCE with NO TRANSFORMATION
	- This lowers the pressure on source; shifts pressure on to data lake.
	- Use of different query engines Presto, Spark and Hive, allowed users to use tools that best addressed their needs, making the platform more flexible and accessible.
	

## My Big Data Project
This project is a means for me to practice building a 'Big Data Platform' that incorporates best practices and design principles that I have learnt in my 2 odd years as a junior Data Engineer. A significant source of inspiration for this project is Uber's Big Data platform and its evolution, both of which you can read about here: https://eng.uber.com/uber-big-data-platform/.

The rough engineering goal with this project is to build an application that provides what I understand to be the full stack of data analytics services, namely, central access to raw data from a variety of sources, access to structured versions of said raw data, visualization & reporting tools based on the housed data and finally, predictive analytics and forecasting based on the same housed data.

An ideal performance target to reach would be a Big Data Platform that is modular enough to be able to work in almost any field of interest. Since my interests are as varied as Physical Strength and Endurance Training, Quantitative Finance, Aerospace Engineering and Meteorology, I want to be able to have access to an analytics platform that is able to service my data needs regardless of my area of interest.

<!---
- 👋 Hi, I’m @pranavathreya
- 👀 I’m interested in Quantitative & Computational Finance, Machine Learning & Software Engineering.
- 🌱 I’m currently studying the book "Hands-On Machine Learning with Scikit-Learn, Keras and TensorFlow".
- 💞️ I’m looking to collaborate at any level on projects involving Big Data, Quantitative & Computational Finance, and ML.
- 📫 You can reach me at pranavsubbu@gmail.com.
--->
<!---
pranavathreya/pranavathreya is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
