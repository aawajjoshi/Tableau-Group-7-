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

The next step is creating worksheets. 



**2. Worksheets**

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

Following the aforementioned steps will produce a worksheet that resembles the worksheet in the picture below.

![ws7](https://user-images.githubusercontent.com/31771293/48374842-a3568880-e68b-11e8-966d-eba6d71f9ff8.png)

Now, we will create another worksheet. Click on the **New Worksheet** button on the bottom navigation bar and rename the new worksheet to *Number of Athletes*. Next, drag and drop the **Name** field from the **Dimensions** on the left hand pane to the **Text** button under the **Marks** section.

![ws8](https://user-images.githubusercontent.com/31771293/48374843-a3568880-e68b-11e8-83bd-3e2bbae8161d.png)

Hover the mouse pointer on the **Name** button to toggle the drop-down arrow and click on it. From the drop-down menu, select **Measure** and change it to **Count (Distinct)**.

![ws9](https://user-images.githubusercontent.com/31771293/48374844-a3568880-e68b-11e8-87c5-4180c702f54a.png)

Following the aforementioned steps, change the shading color of the worksheet. Rename the header to *Number of Athletes* and alter the font color to white, and centrally align the header. Similarly, change the shading color of the title, centrally align the text, and alter the font size to 28. The new worksheet should resemble the one shown in the picture below.

![ws10](https://user-images.githubusercontent.com/31771293/48374845-a3568880-e68b-11e8-99aa-bdb8c678b621.png)

Now, lets create a third worksheet called *Gold Medals*. To create a new measurement for the worksheet click on **Analysis** on the top navigation bar and select **Create Calculated Field**.

![ws11](https://user-images.githubusercontent.com/31771293/48374846-a3568880-e68b-11e8-8447-0a4d2aca2435.png)

From the pop-up box that appears on-screen, change the title to *Number of Gold Medals*. Inside the calculation box, type in the following:
```
IF [Medal] = "Gold"
THEN 1
END
```
If the calculation is valid then a feedback will appear stating *The calculation is valid*. Then, click on apply. 

![ws12](https://user-images.githubusercontent.com/31771293/48374847-a3ef1f00-e68b-11e8-96e8-0924d1d3d8c0.png)

Next, drag and drop the **Number of Gold Medals** under the **Measures** section from the left side pane to the **Text** button on the **Marks** section. 

![ws13](https://user-images.githubusercontent.com/31771293/48374863-acdff080-e68b-11e8-90a5-e617d6d7a3c0.png)

Following the aforementioned steps, change the shading color of the worksheet. Rename the header to *Number of Gold Medals* and alter the font color to white, and centrally align the header. Similarly, change the shading color of the title, centrally align the text, and alter the font size to 28. The new worksheet should resemble the one shown in the picture below.

![ws14](https://user-images.githubusercontent.com/31771293/48374864-acdff080-e68b-11e8-9c62-134ec09ba7f0.png)

Next, we will create another worksheet titled *Gender*. Drag and drop the **Name** field under the **Dimensions** section from the left side pane to the **Columns** box in the worksheet. If a *Warning* pop-up box shows, select **Add all members**. Hover the mouse pointer on the **Name** button to toggle the drop-down arrow and click on it. From the drop-down menu, select **Measure** and change it to **Count (Distinct)**.

![ws15](https://user-images.githubusercontent.com/31771293/48374865-acdff080-e68b-11e8-8099-068c9f3ce70f.png)

Drag and drop the **Sex** field under the **Dimensions** section from the left side pane to the **Rows** box in the worksheet.

![ws16](https://user-images.githubusercontent.com/31771293/48374866-acdff080-e68b-11e8-89f5-23461323f3f5.png)

Drag and drop the same **Sex** field under the **Dimensions** section from the left side pane to the **Colors** button under the **Marks** section. The new worksheet should resemble the one shown in the picture below.

![ws17](https://user-images.githubusercontent.com/31771293/48374867-acdff080-e68b-11e8-94d7-45cb7109f2d7.png)

Finally, create the last worksheet titled *Olympics Data by Region*. Double clikcing on the **Regions** field under the **Dimesions** section on the left side pane will generate a map in the new worksheet. 

![ws18](https://user-images.githubusercontent.com/31771293/48374868-acdff080-e68b-11e8-8ed9-b3ef1ba1bbe5.png)

Drag and drop the **Name** field under the **Dimensions** section from the left side pane to the **Color** button under the **Marks** section. If a *Warning* pop-up box shows, select **Add all members**. Hover the mouse pointer on the **Name** button to toggle the drop-down arrow and click on it. From the drop-down menu, select **Measure** and change it to **Count (Distinct)**.

![ws19](https://user-images.githubusercontent.com/31771293/48374883-b6695880-e68b-11e8-8533-76c3741dd259.png)

Drag and drop the **Medal** field under the **Dimensions** section from the left side pane to the **Tooltip** button under the **Marks** section. Hover the mouse pointer on the **Medal** button to toggle the drop-down arrow and click on it. From the drop-down menu, select **Measure** and change it to **Count (Distinct)**. The final worksheet should resemble the one shown in the picture below.

![ws20](https://user-images.githubusercontent.com/31771293/48374884-b701ef00-e68b-11e8-998b-aa9f5b6b874a.png)

The next step is creating a dashboard. 



**3. Dashboard**

To create a new dashboard, click on **New Dashboard** icon next to the **New Worksheet** icon on the bottom navigation bar. To rename a worksheet, double click on that worksheet tab or right click on the tab and select **Rename**.

![db1](https://user-images.githubusercontent.com/31771293/48379750-d5bbb200-e69a-11e8-81bd-b773da6d4330.jpg)

The left side pane of the new dashboard lists all the sheets under the **Sheets** section. Select the *Olympics Data by Region* worksheet and drag it to the empty dashboard canvas.

![db2](https://user-images.githubusercontent.com/31771293/48379751-d5bbb200-e69a-11e8-8f4b-9415b4c8a939.jpg)

Following the aforementioned steps will produce a dashboard canvas that resembles the one in the picture below.

![db3](https://user-images.githubusercontent.com/31771293/48379752-d5bbb200-e69a-11e8-8b0f-740f0699c934.jpg)

Next, select the *Gender* worksheet and drag it to the dashboard canvas and hold the mouse button until a rectangular outline appears on the lower half of the canvas. Then, let go of the mouse button to release the worksheet within the rectangular box. Following the aforementioned steps will produce a dashboard canvas that resembles the one in the picture below.

![db4](https://user-images.githubusercontent.com/31771293/48379753-d6544880-e69a-11e8-9880-e9a280fd7c4b.jpg)

Drag the rest of the worksheets under the *Gender* section in the dashboard. Initially, the worksheets may appear misaligned as shown in the picture below.

![db5](https://user-images.githubusercontent.com/31771293/48379754-d6544880-e69a-11e8-97e6-07a31e005321.jpg)

To fix this issue, right click on one of three sheets to bring up a pop-up menu and select **Fit Width** under **Fit**. Do the same to properly align the remaining two worksheets.

![db6](https://user-images.githubusercontent.com/31771293/48379755-d6544880-e69a-11e8-857f-6b2c7572c67f.jpg)

Once the widths are fixed, hover the mouse pointer on the edge of a sheet to toggle the resize arrow. Click and drag the arrow to resize the sheets on the dashboard.

![db7](https://user-images.githubusercontent.com/31771293/48379821-0dc2f500-e69b-11e8-94a8-0740e537b84a.jpg)

To reduce the space that the filters are taking up on the right side of the dashboard, click on the purple-scaled filter that may have a title similar to *Distinct count of names* to toggle a grab bar. Click and drag the filter to a different location within the sheet using the grab bar.

![db8](https://user-images.githubusercontent.com/31771293/48379822-0dc2f500-e69b-11e8-8da7-11b9fc28b0ae.jpg)

Place the filter directly underneath the map.

![db9](https://user-images.githubusercontent.com/31771293/48379817-0d2a5e80-e69b-11e8-94c1-80f61b38c19b.jpg)

Following the aforementioned steps will leave one filter behind. This filter is not required and can be removed by clicking on it to toggle an inversed traingle icon to produce a drop-down box and selecting **Remove from Dashboard**.

![db10](https://user-images.githubusercontent.com/31771293/48379818-0d2a5e80-e69b-11e8-8773-6d55c4a647f4.jpg)

Create additional filters for the dashboard to filter the data by season, by sport, and by year. Click on the *Olympics Data by Region* worksheet tab on the bottom navigation bar to open the worksheet. Then, drag and drop **Year**, **Sport**, and **Season** into the **Filters** section which is located directly above the **Marks** section.

![db11](https://user-images.githubusercontent.com/31771293/48379819-0d2a5e80-e69b-11e8-9195-c99a09e0601d.jpg)

Next, click on the map on your dashboard to toggle the inverted triangle icon on its upper right side corner. Click on the icon and select **Filters** to ensure that the three filters have been added.

![db13](https://user-images.githubusercontent.com/31771293/48379842-216e5b80-e69b-11e8-8da2-a37a737fdd65.jpg)

Click on each of the three filters to add them to the dashboard. Following the aforementioned steps will produce a dashboard that resembles the one in the picture below.

![db14](https://user-images.githubusercontent.com/31771293/48379843-216e5b80-e69b-11e8-84f1-3fea02129988.jpg)

The filters pane will initially apper very messy because all the filter options are expanded. To implement a visually cleaner look, click on a filter to toggle the inverted triangle icon. Click on the icon and select **Single value (dropdown)** to make use of a drop-down selection format. 

![db15](https://user-images.githubusercontent.com/31771293/48379844-216e5b80-e69b-11e8-9203-5b30687d9343.jpg)

Repeat the step for the remaining two filters. To place them in a more central and easily accessible area of the dashboard, drag each of the three filters to the map portion of the dashboard and hold the mouse button until a rectangular outline appears. Let go of the mouse button to release the three filters within the rectangular box.

![db16](https://user-images.githubusercontent.com/31771293/48379845-2206f200-e69b-11e8-9ff9-c391099c9c7b.jpg)

Adjust the size of each filter box as desired. Arrange them side-by-side for easy accessibility as shown in the picture below. 

![db17](https://user-images.githubusercontent.com/31771293/48379846-2206f200-e69b-11e8-919c-e317471d4c9a.jpg)

To apply a filter, click on the dropdown arrow and select **All Using This Data Source** under **Apply to Worksheets**. This option will apply a filter to all the worksheets on the dashboards.

![db18](https://user-images.githubusercontent.com/31771293/48379847-2206f200-e69b-11e8-86ce-e914edeb1ad5.jpg)

To view your dashboard in presentation mode, select **Windows** on the top navigation bar and then **Presentation Mode**.

![db19](https://user-images.githubusercontent.com/31771293/48379848-2206f200-e69b-11e8-8569-5ae042119138.jpg)

Following the aforementioned steps will produce a dashboard that resembles the one shown in the picture below.

![db20](https://user-images.githubusercontent.com/31771293/48379849-2206f200-e69b-11e8-885e-b23b93a19ff5.jpg)



**4. Stories**

Click on the **New Story** icon besides the **New Dashboard** icon on the bottom navigation bar to create a story. Drag and drop each sheet to the top half of the window (besides **Add a Caption**) to create a story from the sheets. It is important that the sheets be dragged to the top window of the story canvas as dragging it to the bottom window will delete the sheet that was previously dragged and dropped and replaced it with the new one. Add a brief caption to each sheet dragge to the window by clicking on **Add a Caption** box. 

Following the aforementioned steps will produce stories that resemble the ones shown in the picture below. 

![st1](https://user-images.githubusercontent.com/31771293/48391929-93ac6380-e6ce-11e8-9d4a-912ee754c05d.png)

![st2](https://user-images.githubusercontent.com/31771293/48391930-93ac6380-e6ce-11e8-972c-cb7467d13000.png)

![st3](https://user-images.githubusercontent.com/31771293/48391931-9444fa00-e6ce-11e8-86b5-47fd6ecb6fb3.png)

![st4](https://user-images.githubusercontent.com/31771293/48391932-9444fa00-e6ce-11e8-9d3e-c99786100aa1.png)

![st5](https://user-images.githubusercontent.com/31771293/48391933-9444fa00-e6ce-11e8-93d4-9a642767da9d.png)


## References 
[Tableau's *Getting Started* video tutorial](https://www.tableau.com/learn/tutorials/on-demand/getting-started?product=tableau_desktop%2Btableau_prep&version=tableau_desktop_2018_3%2Btableau_prep_2018_2_1&topic=getting_started)

[Dataset obtained from Kaggle](https://www.kaggle.com/heesoo37/120-years-of-olympic-history-athletes-and-results/home)

[Tutorial Point's free *Learn Tableau* guide](https://www.tutorialspoint.com/tableau/)

[Udemy's *Tableau Tutorial for Beginners* course](https://www.udemy.com/tableau-tutorial-for-beginners/)

[Edurek'a *Tableau Training for Beginners* series on YouTube](https://www.youtube.com/watch?v=jj6-0cvcNEA)

[Tableau discussions on Stack Overflow](https://stackoverflow.com/questions/tagged/tableau)


## Authors 

**Anusha Chowdary Kollu**  
**Elizebeth Conard**  
**Sierra King**   
**Aawaj Raj Joshi**

