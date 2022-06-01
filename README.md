# Automation of Storage of Different Dataset Versions

![blog](https://user-images.githubusercontent.com/95134445/171471153-3a3ede4a-b3e2-4840-b47a-81abdab6671d.gif)

Using **Github Actions**, we automate the runs of a Jupyter notebook (Here I have taken automatic update intervals of 1 hr on 1st and 2nd June as indicated by my cron job) to generate a csv file containing the updated data.

An **example usecase** is if we have a dataset on topics such as weather, cryptocurrencies, stock market, COVID-19 stats etc. which update over time, we can store the hour wise, day wise, week wise etc. updated versions of the data for further analysis for a particular time period or time series analysis etc. This github action helps automate that process and stores all the data in the data folder

**Currently using a toy dataset** 

**Update done to File Handling System @ 22:26 IST, 1st June :** I noticed file names clashing due to earlier naming system so now the file name uses the date and the fact that (60xhour + minute) value will never be same for hourly updates in a day.

References:
1. https://crontab.guru/#0_*/1_1-2_6_*
2. https://github.com/actions/starter-workflows
3. https://github.com/actions/setup-python
4. https://github.com/marketplace/actions/run-notebook
5. https://raw.githubusercontent.com/quantumsnowball/toy-datasets-collections/master/titanic/titanic.csv
6. ...
