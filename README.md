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

https://github.com/aawajjoshi/Tableau-Group-7-/blob/master/AthleteEvents.xlsx

## Overview of our project

In this project, we explore a few different things you can accomplish with a dataset using Tableau, namely creating graphical visualizations on a worksheet, producing an interactive dashboard, and conveying your message through a rich story. 

## Step-by-step instructions 

**1. Getting Started**

After the installation is complete, run the Tableau Desktop application. A fresh startup will load into the *Start Screen*. The pane on the left hand side of the *Start Screen* is the *Connect Pane*. Since we are working with an excel datasheet, we will select **Microsoft Excel** option listed under **To a File**. 

![gs1](https://user-images.githubusercontent.com/31771293/48342461-547e0400-e635-11e8-8ce4-a2f6c7c6a09e.PNG)

In the pop-up window, navigate to where you saved the downloaded dataset and double click the file to open it. 

Successful processing of the dataset will lead to the *Data Source* page. Double click on **New Union** in the *Connections* pane which is on the left hand side of the *Data Source* page. 

![gs2](https://user-images.githubusercontent.com/31771293/48342632-d3733c80-e635-11e8-8ee5-38d8761e6bde.png)

Drag and drop the three excel sheets (First 3rd, Middle, Last 3rd) into the pop-up box and click 'Apply' to create a Union of our three datasheets.

![gs3](https://user-images.githubusercontent.com/31771293/48342676-f69dec00-e635-11e8-8ea6-bfa81d4572a2.png)

Select **Automatic Update** to ensure that the data will be automatically updated after each change. 

![gs4](https://user-images.githubusercontent.com/31771293/48342776-38c72d80-e636-11e8-8867-d9ab84144d93.png)

Now, drag and drop the Region Key from the *Connections* pane besides the Union we created to establish an inner join. This creates a join between the regions in the Region sheet and the region keys in the other three sheets. 

![gs5](https://user-images.githubusercontent.com/31771293/48342958-ac693a80-e636-11e8-95c5-da46ba7ac323.png)

In order to make the regions concise in the world map that we will be generating later, we need to change the data format of Region column. Click on **Abc**, and under **Geographic Role**, select **Country/Region**. This will change the **Abc** into an icon of a globe.

![gs6](https://user-images.githubusercontent.com/31771293/48343202-62348900-e637-11e8-819e-1ccd77d6b6cf.png)

![gs7](https://user-images.githubusercontent.com/31771293/48343212-695b9700-e637-11e8-9fd6-907696d0e439.png)

Next, we will look at WorkSheets.

2. WorkSheets

You can rename the worksheet by double clicking on the tab. For the first worksheet rename it Average Age. On the left under the Measures sections you will see Age. Drag and drop Age to the Text Icon in the Marks section. You should see this: 


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

