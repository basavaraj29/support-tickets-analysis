# support-ticket-analysis
A Statistical overview of the Support Tickets data at GCDO, IBM.

## Table of Contents
1. [Dependencies](#deps)
2. [Project Motivation](#motivation)
3. [File Descriptions](#desc)
4. [Results](#results)
5. [Licensing, Authors, Acknowledgements](#licensing)

## Dependencies<a name="deps"></a>
Pandas 1.0.1, numpy 1.17.4, scikit-learn 0.20.0
The code is developed using python3 (3.7.0), and the above libraries. It should mostly run on a different version of the above libraries too.

## Project Motivation<a name="motivation"></a>
The IBM Global Chief Data Office (GCDO) is a world-wide team of highly skilled engineers, who develop and maintain the
key initiatives that drive IBM's Data and AI transformation.

In the GCDO, we have the Cognitive Enterprise Data Platform (CEDP) that serves as the backbone for data and AI processes
across the IBM enterprise. Previously siloed data, converges onto one platform and provides a reliable data source.

CEDP offerings consist of various tools and frameworks. It has a dedicated support team to address concerns/issues on
all of its offerings. CEDP Support team uses Jira for issue/ticket tracking and resolution.

For this project, I was interested in exploring a few trends of CEDP Support Tickets for a period of 30 months since
initiation of the project. The data is proprietary to IBM, and hence I've uploaded only anonymised sample data of 10
rows.

1. Average resolution time for a ticket. How has it progressed over time? How is the distribution?
2. Busiest hours of the day, week. Monthy patterns among tickets raised
3. Correlation of the resolution time with other factors.
4. Prediction of ticket labels from the ticket summary.

## File Descriptions<a name="desc"></a>
There is one notebook file `jira_data_analysis.ipynb`. If you wish to test this, please execute the last 3 cells.
In the last three cells, the pre-trained model is loaded and executed on test data.

File `classifier.pkl` is where the trained model is stored. `jira.csv` contains anonymised sample data.

## Results<a name="results"></a>
The main findings of this study can be found [here](https://medium.com/@basavaraj_42993/a-statistical-overview-of-the-support-tickets-data-at-gcdo-ibm-f7ed55bc208e). The `jira_data_analysis.ipynb` file has cells explaining  
answers/trends for each of the questions above.

## Licensing, Authors, Acknowledgements<a name="licensing"></a>
Credits to CEDP Support team for providing me access to the data. The data is proprietary to IBM. The sole purpose of
the project is to demonstrate few trends in the Ticket data. Without proper authorisation, the code/model should not be
used elsewhere.
