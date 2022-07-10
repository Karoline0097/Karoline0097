# 🌱 About Me 
Welcome on my profile! 
I am Karoline, about to finish my studies in Medicine. My desire for innovative thinking and developing led me to discover my passion for programming. My current hands-on software project as a working student further encourages me to dive deeper into IT/ Software Development. I am curious to learn more about software, data and programming to solve real-world problems as part of a diverse team. 

# (Self) Learning Progress since 02/22 with:
#  Hands On Project: 
Working Student in Software Development [@Finepower Gmbh](https://www.finepower.com/)
#  Online Resources:
* [University of Minnesota: Software Development Lifecycle](https://www.coursera.org/specializations/software-development-lifecycle?) (Currently enrolled)
* [Tutorials on Software Design](https://www.youtube.com/playlist?list=PLjtYWQ9arEeoQXFb5hCNQsJe21fN9gXM8), [ArjanCodes](https://www.youtube.com/c/ArjanCodes)
* [Tutorials on Object Oriented Programming](https://www.youtube.com/playlist?list=PLjtYWQ9arEer1pn0J8rLKqAX2ywhaxP1P)
* [Tutorials on Data Structures & Algorithms](https://www.youtube.com/playlist?list=PLjtYWQ9arEeplkZbRAkAOCXI0AWTjXMDy)
* [Tutorials on SQL, Databases, DBMS](https://www.youtube.com/playlist?list=PLjtYWQ9arEepgFfGrMu356RK3VUc2jRqM)
* [Tutorials on APIs](https://www.youtube.com/playlist?list=PLjtYWQ9arEera8NdZtcqHyrc9sg97E6Qf)
* [Tutorials on UIs](https://www.youtube.com/playlist?list=PLjtYWQ9arEer8BWPit7a1XXUgxax-0Dem)
* [Tutorials on Python Programming](https://www.youtube.com/playlist?list=PLjtYWQ9arEeroYETt-jVWow2mX-enhrsZ)
* [Tutorials on VCS (Git) & IDEs](https://www.youtube.com/playlist?list=PLjtYWQ9arEepuevbWPhrMyBvn8IR41IQM)
* [MITx: Introduction to Computer Science and Programming Using Python 6.00.1x ](https://www.edx.org/course/introduction-to-computer-science-and-programming-7) (Successfully completed)
* [University of Michigan: Python for Everybody](https://www.coursera.org/specializations/python) (Successfully completed)

# Programming Languages
* Python 

# Relational Databases (SQL)
* DBMS: SQLite, MySQL
# Non-Relational Databases (NoSQL)
* JSON, XML

# My Projects:

## Bill of Material (BOM) Application [@Finepower Gmbh](https://www.finepower.com/): 
* [Private Repository](https://github.com/Karoline0097/BOM_finepower/blob/main/README.md) from my working student job [@Finepower Gmbh](https://www.finepower.com/)
* Private Repository, code & application can be presented & explained via screenshare

### Development of an in-house application for process optimization
* Automate search, managment and order of hundreds of PCB components for PCB prototype assembly with big hardware suppliers Mouser and Farnell 
* Optimized for current supply shortages of power electronic products

### Requirements
* PCBs are designed by hardware engineers using a pcb software (Eagle). For each electric component on this PCB, an appropriate manufacturer part number that fulfills the requirements for the component is choosen by the hardware engineer. Before PCB prototype assembly in the company, a bill of material (BOM) with all electric components with those manufacturer part numbers  is created. For each item on the BOM, a product must be choosen and ordered from hardware supplier online shops (Mouser, Farnell...).
* Problem to solve: 
Manual search of all products by the hardware enigneer and creation of carts by the office manager are very time-consuming processes. Especially now due to current supply shortages in the hardware industry, a considerable amount of working time is spent searching the online shops of hardware suppliers repeatedly for every component on the PCB.
### Functional Requirements
* User Groups: Hardware Engineers, Office Manager
* Application Period: Between completion of PCB Design and before PCB prototype assembly
*	Several hardware engineers work together on the same PCB. Therefore, the BOM inside the application will be created, edited and contributed to by multiple users over a period of time. The application should keep track of sources of manufacturer part numbers and relevant changes to a BOM (with a timestamp and user responsible for the action).
* A BOM consists of many PCB components, for each of witch a manufacturer part number is predefined by the hardware engineer inside the PCB design software. All products for each of those manufacturer part numbers should be searched with hardware suppliers, displayed in an user-friendly way and saveable for later work (with the same or another user).
*	When a product is available for order and its manufacturerer part number exactly matches part number from csv/user, it should be preselected, else nothing should be preselected
*	visually display / give quick overview over all available product options
*	prevent false orders
*	send all choosen products, ready to order, to office assistant who orders created carts
*	user can manually add other part options that he judges are appropriate alternatives for a pcb component
*	users can remove part options from csv/user if they judge them to be inappropriate
* all product order choices are made by user

### Process/ System Design Requirements
* IDE: PyCharm Community Edition
* Programming Language: Python
* Database: SQLite (serverless SQL DBMS)
* Libraries: must all be Open Source
* Development Method: OOP, FP

### Software Architecture: Layered Model
* UI
* Application Logic
* SQL Relational Database & SQLite DBMS
* Mouser and Farnell Web APIs (JSON)
* [Mouser API](https://www.mouser.de/api-hub/)
* [Farnell API](https://partner.element14.com/docs/Product_Search_API_REST__Description)

### Screenshots of BOM Tool:

* Work with csv and db files 
![CSV and DB Files](https://user-images.githubusercontent.com/96637498/177588030-42104065-5d29-445b-a463-ef1fa149d429.png)

* Search & Update Product Results from Mouser & Farnell APIs
* choose a product for order with pulldown menu
* visually display status of choosen product
![Bildschirmfoto 2022-07-06 um 17 26 01](https://user-images.githubusercontent.com/96637498/177594821-d4ac3a4b-acd2-4e38-815d-d1a17e2cd510.png)

* view more information on a PCB Component (related Part Options, Search Results...)
![Bildschirmfoto 2022-07-06 um 17 26 10](https://user-images.githubusercontent.com/96637498/177594924-ee55dab0-7e6d-40a9-bb8f-2cfaa20d37a3.png)
![Bildschirmfoto 2022-07-06 um 17 26 44](https://user-images.githubusercontent.com/96637498/177594007-a47b37da-3cfa-459a-95d4-a3c8dfd51a7e.png)

* manually add own part options for a pcb component
* this function provides more flexibility which is needed due to current supply shortages
![Bildschirmfoto 2022-07-06 um 17 27 51](https://user-images.githubusercontent.com/96637498/177589106-9271a5dd-f940-447c-b4e4-85c44775dab3.png)

* keep track of actions performed by your colleagues via comment section and action log
![Bildschirmfoto 2022-07-06 um 17 28 33](https://user-images.githubusercontent.com/96637498/177589303-9184ce3b-9d5b-4fd6-9fe2-925db79d00f4.png)

* automaticaaly create carts with Mouser and Farnell APIs
![Bildschirmfoto 2022-07-06 um 17 28 54](https://user-images.githubusercontent.com/96637498/177595020-bec0fd84-4b30-4137-95f7-cadba468dd82.png)



## Online Courses and Projects: 
* [Repository](https://github.com/Karoline0097/Introduction-to-Computer-Science-and-Programming-Using-Python) from my participation in [MITx Introduction to Computer Science and Programming Using Python 6.00.1x ](https://www.edx.org/course/introduction-to-computer-science-and-programming-7)
* [Repository](https://github.com/Karoline0097/University-of-Michigan-Python-for-Everybody) from my participation in [University of Michigan Python for Everybody](https://www.coursera.org/specializations/python)
* Currently enrolled: [Software Development Lifecycle](https://www.coursera.org/specializations/software-development-lifecycle?)


## Learning Interests:
* Software Development Life Cycle
* Software Engineering
* UI Design, Frontend Development
* APIs
* Relational Databases, PostgreSQL, MySQL
* Data Analysis
* C#
...


## Bio:
* since 2022: Working Student @Finepower GmbH Munich
* 2021-22: Ovarian Cancer Research and Tumor Database @LMU Munich Medical Research School @LMU Hospital
* 2016-22: Medical Studies @LMU Munich








<!---
Karoline0097/Karoline0097 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
