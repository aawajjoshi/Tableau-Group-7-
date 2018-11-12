# Tableau (Group 07)

Tableau is a powerful business intelligence tool that allows users to visually analyze their data. It is a secure and flexible end-to-end analytics platform that enables individuals and businesses to devise interactive and shareable dashboards that allows for study of trends, variations, and density of data in the form of visually apealling interactive visualizations like graphs and charts. Tableau is easy learn, thanks to their implementation of a simple, yet powerful drag-and-drop feature. The platform allows for real-time collaboration, easy connection to big data sources, and even supports the Hadoop platform. 

## Download Tableau

Click on the link below to dowload Tableau (free for students). After the download is complete, open the installation file and follow the on-screen instructions to install Tableau Desktop on your computer. 

https://www.tableau.com/academic/students

## About our dataset 

Our historical dataset concerns Olympic athletes and medal results spanning twelve decades, specifically from 1896 Olympics in Athens to the 2016 Olympics in Rio de Janeiro. A unanimous decision was made by the team to divide the huge Excel sheet into three smaller sheets in order to showcase Tableau's **Union** and **Join** features. 

## Link to our dataset 

We obtained our dataset on [Kaggle](https://www.kaggle.com/). Here is the link to the raw dataset. 

https://www.kaggle.com/heesoo37/120-years-of-olympic-history-athletes-and-results/home

We have added the partioned version of the dataset to our repository. Here is a direct link to the file on our repo. 





## Steps 
After the installation is complete, run the Tableau desktop application. When the application loads, select 'Microsoft Excel' under 'Connect' and 'To a File' since we are working with excel datasheet. 

After the datasheet is processed, double-click on 'New Union' to open the Union pop-up. Drag and drop the three excel sheets (First 3rd, Middle, Last 3rd) and click 'Apply' to create a Union of our three datasheets. Click automatic update. 

Drag and drop the Region Key besides the Union to create an inner join. Region gets added to the datasheet along with the already present Region Key. As we are using maps in our sheets, to make the region clear, click on the 'Abc' and select Geographic Role, then select Country/Region. Then click on Sheet1 on the bottom navigation bar to bring up your new empty worksheet. You can rename the worksheet by double clicking on the tab. For the first worksheet rename it Average Age. On the left under the Measures sections you will see Age. Drag and drop Age to the Text Icon in the Marks section. You should see this: 


Click on the New Story icon besides the New Dashborad icon to create a story. Drag and drop each sheet to the top half of the window (besides 'Add a Caption') to create a story from our sheets. It is important that we drag each of the sheets to the top window because if we drag and drop it on the bottom window, it will replace the sheet you dragged prior to the new one. You can add a bief caption to each sheet you drag to the window by clicking on 'Add a Caption'. The caption is simply a story about the sheet. 

If you followed all the aforementioned steps, your story should look something like this. 

## References 
Kagle
Tableau's video 


## Authors 

**Anusha Chowdary Kollu**  
**Elizebeth Conard**  
**Sierra King**   
**Aawaj Raj Joshi**

