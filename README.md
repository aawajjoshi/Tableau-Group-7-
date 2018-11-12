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

Next, we will create a worksheet.

**2. Worksheet**

A worksheet titled *Sheet1* should have been automatically created in the bottom navigation bar. If not, clicking on the **New Worksheet** icon next to the **Data Source** button on the bottom navigation bar will generate a new worksheet. To rename a worksheet, double click on that worksheet tab. Following the aforementioned step, rename the first worksheet to *Average Age*. To dive into the data, simply drag and drop the **Age** field located under **Measures** in the left hand pane to the **Text** icon under the **Marks** section.

![ws1](https://user-images.githubusercontent.com/31771293/48374784-802bd900-e68b-11e8-8c31-e9650022cfdd.png)

By default, the worksheet will generate the total sum of ages. Since, we seek the average age, hover the mouse pointer on the **SUM(Age)** button to toggle the drop-down arrow. Click on the arrow to produce a drop-down box. In the drop-down box, select **Measure** and then **Average** to generate the average age of the Olympic athletes. 

![ws2](https://user-images.githubusercontent.com/31771293/48374796-8752e700-e68b-11e8-89f2-ff8971e42e1f.png)

To change the background color of the worksheet, click on **Format** at the top navigation bar and select **Shading**. *Format Shading* pane will pop-up on the left hand side of the screen. The worksheet background color can be altereted in the **Worksheet** drop-down selection under **Default**.

![ws3](https://user-images.githubusercontent.com/31771293/48374806-8c179b00-e68b-11e8-8da5-782c33e68005.png)

To change the header, double click on the default *Sheet 1* header to bring up a pop-up box that allows formatting. Change the header from *Sheet 1* to *Average Age*, align the header on the center of the sheet, and change the font color to white.

![ws4](https://user-images.githubusercontent.com/31771293/48374820-95a10300-e68b-11e8-920a-2559fba246aa.png)

To change the background of the header section, right click on it and select **Format Title**. *Format Title and Caption* pane, which will show up on the left hand side of the screen, gives the option to change different attributes of the header section.

![ws5](https://user-images.githubusercontent.com/31771293/48374821-95a10300-e68b-11e8-8dfa-8f3b9b60f038.png)

To alter the attributes of the main text, click on the **Text** button under the **Marks** section. From the pop-up box, align the text in the center of the screen. To change the font size of the text, click on the **...** button. Change the font size to 28. 

![ws6](https://user-images.githubusercontent.com/31771293/48374822-95a10300-e68b-11e8-9d79-914f3091de61.png)


![ws7](https://user-images.githubusercontent.com/31771293/48374842-a3568880-e68b-11e8-966d-eba6d71f9ff8.png)
![ws8](https://user-images.githubusercontent.com/31771293/48374843-a3568880-e68b-11e8-83bd-3e2bbae8161d.png)
![ws9](https://user-images.githubusercontent.com/31771293/48374844-a3568880-e68b-11e8-87c5-4180c702f54a.png)
![ws10](https://user-images.githubusercontent.com/31771293/48374845-a3568880-e68b-11e8-99aa-bdb8c678b621.png)
![ws11](https://user-images.githubusercontent.com/31771293/48374846-a3568880-e68b-11e8-8447-0a4d2aca2435.png)
![ws12](https://user-images.githubusercontent.com/31771293/48374847-a3ef1f00-e68b-11e8-96e8-0924d1d3d8c0.png)
![ws13](https://user-images.githubusercontent.com/31771293/48374863-acdff080-e68b-11e8-90a5-e617d6d7a3c0.png)
![ws14](https://user-images.githubusercontent.com/31771293/48374864-acdff080-e68b-11e8-9c62-134ec09ba7f0.png)
![ws15](https://user-images.githubusercontent.com/31771293/48374865-acdff080-e68b-11e8-8099-068c9f3ce70f.png)
![ws16](https://user-images.githubusercontent.com/31771293/48374866-acdff080-e68b-11e8-89f5-23461323f3f5.png)
![ws17](https://user-images.githubusercontent.com/31771293/48374867-acdff080-e68b-11e8-94d7-45cb7109f2d7.png)
![ws18](https://user-images.githubusercontent.com/31771293/48374868-acdff080-e68b-11e8-8ed9-b3ef1ba1bbe5.png)
![ws19](https://user-images.githubusercontent.com/31771293/48374883-b6695880-e68b-11e8-8533-76c3741dd259.png)
![ws20](https://user-images.githubusercontent.com/31771293/48374884-b701ef00-e68b-11e8-998b-aa9f5b6b874a.png)



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

