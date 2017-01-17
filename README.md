**INTRODUCTION** 

oHealth Context is an initiative proposed as part of the SmartSDk project track HealthCare-App. Its aims is to benefit a range of individuals and organizations (e.g., patients, researchers, health care system, government, etc.) by reducing the complexity of health data, through a standardized set of schemas and software stack that might facilitate writing applications that can process and create clinical data, regardless of where the data comes from.

The interpretation of clinical data is critical and needs to be associated to proper metadata. For instance, it is imperative for a physician to differentiate between glucose levels among diabetic patients, or to distinguish whether a heart patient is self-reporting his heart rate or whether it is being automatically collected during resting or exercise time. In this context, oHealth Context provides useful data structures to facilitate a meaningful interpretation of the data. 

oHealth Context is built based on an open source health set of specifications called: Open mHealth; which consist on a set of tools and specifications designed to handle medical data. 

**SCHEMAS**

Data schemas specify the format and content of data, such as blood glucose readings, blood pressure, body fat percentage, calories burned, among others; which affects how pre-defined programs might compute data. On the other hand, data usually comes from different devices and/or platforms, which enrich but difficult a more interesting across-data analysis. Thus, a common schema serves as a single source of documentation that can be referenced whenever and wherever the data points are used.

The schemas defined in this document are meaningful in distinctions for each clinical measure; for instance, to sense heart rate data, blood pressure, sugar level, so forth, increasing the overall clinical utility of digital health data and improving the ability of developers to quickly build clinically usable outcomes. As proof of concept, we have developed a mobile phone application, named 3Ollin-Test. Thus, we have defined a reduced and specific sets of schemas aimed at measuring the risk of fall for an older adult; as described next.
