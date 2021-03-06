# GE_Data_Analytics_Virtual_Experience_Program(in Tableau)
This is a virtual experience program, not a real internship, but I act as a data scientist in GE Aviation team to gain insights from dataset. The link to my [Certificate of Completion](https://insidesherpa.s3.amazonaws.com/completion-certificates/General%20Electric%20%28GE%29/ThbphD5N5WRsd9Mxo_General%20Electric_NorEhdj87k7nLnwK2_1642265716865_completion_certificate.pdf).

### The program background is:

At GE Aviation, they use the concept of a “Data Lake”. A Data Lake is a single database instance that contains data from all around Aviation. Everything from financial, delivery (of parts and engines), supplier, engine data, customer data, and so on.

The advantage of a Data Lake is that allows the developer to make a single connection string to the Data Lake, and as long as the developer has permissions to see the data – they are able to immediately start creating data-driven insights in a centralized repository of data.

### My task:

In order to assist the GE Aviation team to make decisions based off real time data, I have to do both data engineering and data visualization to drive meaningful insights using enterprise-grade technology.

### 1. Data Engineering

Create a single data set that combines all the data listed below into a single table:

- Flight data (so data relating to the health of the mechanical engine of a plane)
- Location Data for airports
- Manufacturing Data (which relate to various airplane parts)
- Manufacturing Bill of material (which tells what engines have been used)

I tried two methods in this step: Excel(vlookup and index+match) & Tableau (union & join)

### 2. Data Visualization
Create data visualization charts in Tableau to 
- make decisions based off real time data
- ensure quality control in our manufacturing process and to determine if the parts we manufacture are made accurately

The Tableau interactive [dashboard](https://public.tableau.com/app/profile/jing.xie1865/viz/Task2_visualization/Dashboard1?publish=yes) I created includes:
- Component Parts Measurement Tracking (whether measurement of the design attribute is whintin acceptable tolerance from the expected nominal value)
- Frequency of airports that GE engines fly into and outof (both bar chart and symbol map)
- Count of flight cycle, avg RUL(Remaining Useful Life) and avg accept_rate(% of parts acceptable) by 4 airline operators

The screenshot as below:
![Screen Shot 2022-01-15 at 10 40 29 PM](https://user-images.githubusercontent.com/88932816/149647534-6e4f4281-bc8a-4e06-9c58-942657d0118f.png)

My findings can be summarized here:
1. The overall accept_rate for each component part is 0.8, while when inspecting the specific part with unique Serial number, 4% of them have accept_rate lower than 0.5(and most of them having accept_rate at 0). Closer monitor and more efforts may have to be placed on these outliers to ensure the safety of airplane operation.
2. Airport WMKK(Malaysia) is the most common airport that GE engines fly into and outof. Furthermore, Southeast Asia is the most common area where GE engines operates, so more resources can be put into this area such as arranging more flight cycles, designing and manufacturing more customized characteristics etc..
3. AXM is the airline operator having most flight cycles, almost twice as many as others, also echoing the second point since AXM is the main operator in Southeash Asia. Considering the large amounts of flight, we could monitor the performance of this operator more carefully, including tracking its capacity and quality closely.

You can also refer to the Tableau interactive dashboard I created [here](https://public.tableau.com/app/profile/jing.xie1865/viz/Task2_visualization/Dashboard1?publish=yes). Hope it helps!
