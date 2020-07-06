# BUILDING A SUCCESSFUL MACHINE LEARNING WORKFLOW
## May 24, 2020
## About RIHAD VARIAWA
> As a Data Scientist and former head of global fintech research at Malastare.ai, I find fulfillment tacking challenges to solve complex problems using data

*Not every client is ready for data science implementation, according to RIHAD VARIAWA. In order to produce real business value, RIHAD recommends spending more time understanding the business problems at hand and what you really want to predict before diving into a solution. When projects are data-science ready, clients’ needs and preferences dictate the technologies used on a case-by-case basis*

![](https://media.giphy.com/media/pqnY0eDsO7nvgHvjSv/giphy.gif)

In a less mature industry like data science, there aren’t always textbook answers to problems. When undertaking new data science projects, *data scientists* must consider the specificities of the project, past experiences and personal preferences when setting up the source data, modeling, monitoring, reporting and more

While there’s no one-size-fits-all method for data science workflows, there are some best practices, like taking the time to set up auto-documentation processes and always conducting post-mortems after projects are completed to find areas ripe for improvement

Ryder Zern, manager at *Malastare.ai*, said he focuses on evaluating the utility and business value of what the team has built

> “More important than any specific tool or technology, is proactively, consciously adopting a mindset that’s focused on continual evaluation and optimization,” Zern said

Data Science Coach Ben Oren of *Flatiron School* agreed on the importance of assessing each project after the fact. Improving data science workflows often occurs at the consolidation step, so after every project, he documents what was done, considers where the problems and inefficiencies crept in, and imagines ways to improve processes for the future

Data scientists tweak their data science workflows to align with what works best for their teams and businesses. What other best practices are they using to optimize their data workflows? Code reviews, collaboration between *data scientists and data engineering* teams and agile environments are just a few examples

## A bit about Malastare.ai technical process for building Machine Learning workflows

It’s important to understand the business problem and frame it in a data science context. We work closely with business stakeholders and the data engineering team to identify, collect and create the data needed. This often requires the use of multiple tools depending on the nature of the data (e.g., SQL, Python, Amazon S3, HDFS cluster and Cloud)

The next phase is data processing and exploratory data analysis (EDA). This is where we explore the available data to gain relevant insights and best approaches moving forward. The insights collected during this phase are then used for model building and tuning where we use a variety of machine learning frameworks and Python packages (Spark, Scikit-learn and TensorFlow)

*Malastare.ai* practices what's call *ethical data science.* We know that data science can result in quick failure without proper planning and preparation. We spend time upfront ensuring our clients are data-science ready, and that their projects will bring value. We help them understand the ramifications of machine learning-based decisions, and avoid bias when building models

We are not afraid to tell our customers that they are not ready for data science implementation if we can’t say with integrity that they have the right level of data maturity, or have identified a project that will bring business value

Sharing *Malastare.ai’s* participation on a client's data science platform setup, it’s important to understand the scale that our client operated at: Their systems are required to process about 4 billion events per hour. Those volume requirements influence the type of tools we leveraged when developing data science workflows

For developing models, we leverage *H2O Driverless AI* quite extensively and leverage *Spark ML* for training data pipelines. We are also experimenting with TensorFlow and are building prototypes with Neo4j for GraphDB. The latter we are using to build a fake news machine learning model. We use Airflow for orchestration, Hive and Impala for data exploration, and Jupyter and Zeppelin notebooks for analytics

In our latest project, we’re building streaming data pipelines with *Apache Flink* and are experimenting with building *H2O Driverless AI RESTful APIs*, which our streaming pipelines will leverage. This creates a great challenge to build not just accurate, but also operationally efficient models in order to support our hourly throughput requirements. We are partnering with experts in the area of streaming and with AWS, which represent great learning opportunities for our teams

## Processes or best practices we at Malastare.ai found most effective in creating workflows that are reproducible and stable?

Everyone wants to implement the *buzzworthy* part of data science: particularly, building and deploying machine learning and Ai into their organization. However, not everyone realizes how critical data preparation and data profiling are to data science success. If your organization is not truly data-science ready, then you are doing a huge disservice to outcomes and your bottom line. Invest time in organizing, cleansing and democratizing your data into *one true source* that provides accurate and reliable information

Once this is done, make sure to go beyond basic exploratory data analysis and get a better understanding of what your data is telling you, and what features you might be able to unlock with some upfront discovery

When building a data product, *Malastare.ai* strive to focus on building the right thing and building it right. We invest in cross-functional collaboration and embrace iterative data development. *Malastare.ai* believe that adopting a champion challenger approach during deployment, model development and production makes a huge difference

We strive to build a better model that outperforms the previous model built. We start this process by researching these topics to expand our technical horizons. Code reviews and design reviews are done throughout the process to maximize the stability of our models

We are not just handling large amounts of data, but are also maintaining several hundred machine learning models. Managing this amount of machine learning models requires automation of the data science workflow. As such, we are persisting models in ModelDBs, maintaining feature development code in GitHub, maintaining automatic monitoring, and creating plenty of dashboards describing the health of the models and systems

We’ve also found that having a designated data engineering group support the data science team to be highly beneficial. The members of the latter group are mostly aspiring data scientists who have a good understanding of data science concepts and are honing their skills in the production of data science models. Our data science engineering group partners closely with our data scientists, educating each other and brainstorming on how to overcome common challenges when developing and deploying machine learning models

Lastly, it is very important to “know” your data, which means exporting model evaluation metrics, monitoring training data, developing ways to detect and respond to shifts in your data, and retaining training data for as long as possible

## Advice Malastare.ai has given to other data scientists looking to improve how they build their workflows?

Spend more time understanding the business problems at hand and what you really want to predict before diving into a solution

It is crucial to maintain an agile and collaborative environment when looking at your workflow and testing hacky solutions with robust, reproducible ones every sprint. The key is to always stay curious, be open to learning, and be able to bounce ideas off cross-functional teams. Doing so boosts the quality and velocity of the data product workflow

Creating a perfect model for a question that might not need to be answered, or for which the information quality is low, won’t bring you the most business value and will likely result in failure. Our advice to machine learning leaders is to make sure strong communication is established within your teams and make it known that we can learn from our mistakes, which will make us more experienced data scientists

![](https://drive.google.com/uc?export=view&id=1i7fzIUxz-oEs8V4uMdoZCQUl51NMrbVz)
