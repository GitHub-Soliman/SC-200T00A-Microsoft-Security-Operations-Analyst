# Module 7 - Lab 1 - Exercise 8 - Create workbooks

## Lab scenario

You're a Security Operations Analyst working at a company that implemented Azure Sentinel. You must design workbooks with advanced visualizations.

### Task 1: Explore Workbooks.

In this task, you will explore the configuration of a workbook.

1. Login to WIN1 virtual machine as Admin with the password: **Pa55w.rd**.  

2. In the Edge browser, navigate to the Azure portal at https://portal.azure.com.

3. In the **Sign in** dialog box, copy and paste in the **Tenant Email** account provided by your lab hosting provider and then select **Next**.

4. In the **Enter password** dialog box, copy and paste in the **Tenant Password** provided by your lab hosting provider and then select **Sign in**.

5. In the Search bar of the Azure portal, type *Sentinel*, then select **Azure Sentinel**.

6. Select your Azure Sentinel Workspace.

7. Select **Workbooks**.

8. Select **Identity & Access**, then select the **View template** button.

9. Review the Identity & Access workbook.

10. In the **Azure Sentinel | Workbooks** area (hint: scroll to the left) select the **Templates** tab.

11. In the Templates tab search for and select **Azure AD Sign-in logs**, then select the **Save** button. 

12. Select the location that is appropriate for your location.  The appropriate location usually defaults.

13. Select the **View saved workbook** button.

14. Select **Edit** in command bar.

15. In the *Sign-ins by Location* area, select **Edit** at the bottom of the grid.

#### To format columns, the Column setting panel provides customization options, do the following:

16. Select the **Column Settings** button in the Query Command bar.

17. In the *Edit column settings* fly-in select the column **Failure Count|Interrupt Count**.

18. Review the settings, including the Column renderer and Color palette.

19. Select the column **Trend**.

20. Review the settings, including the Column renderer and Color palette.

21. Select **cancel**.

#### To have one tile/grid control filter the results in another tile/grid do the following:

22. Select the **Advanced Settings** tab in the Query.

23. Review the *When items are selected, export parameters* setting.  Notice the *LocationDetail* field is selected.

24. Select **Done Editing** at the bottom of the query.

25. Select **Edit** for the Device Sign-in details table on the right side of the screen.  

26. In the query, locate "LocationDetails".  The query is using the parameter exported from the other query to filter results.

27. Select **Done Editing** for the query.

28. Select **Done Editing** for the workbook.

### Task 2: Create a Workbook.

In this task, you will create a new workbook with advanced visualizations.

1. Select **Workbooks** in the Azure Sentinel portal.

2. Select **+ Add workbook**

3. Select **Edit**

#### Edit Header text:

4. Change *New workbook* to *My workbook*.

5. Select **Done Editing**.

6. Select **Edit** for the only visible graph.

7. Review the KQL statement that provides a union of counts across multiple tables.

8. Select the **Done Editing**.

9. Select **...** next to the graph area, then select **+ Add**, then select **Add query**.

10. Enter *SecurityEvent* into the query box, then select the **Run Query** button.

11. Change the Time Range to **Last 3 days**.

12. Change the Visualization to different options and see the results.

13. Change the Visualization to **Time chart**.

14. Select **Style** from the Query tab.

15. Select the **Make this item a custom width** box.

16. Set the Percent width to **75** and Maximum width to **75**.

17. Select **Advanced Settings** from the Query tab.

18. Select **Show refresh icon when not editing** box. 

19. Select **Done Editing**.

20. Select **Add**, then **Add query**.

Enter the following KQL command for the query:

```
SecurityEvent
```

21. For Time Range, select **Last 4 hours**.

22. Change the Visualization to **Grid**.

23. Select the **Style** tab.

24. Select **Make this item a custom width**.

25. Change percentage width to **25** and maximum width to **25**. 

26. Select **Done Editing** for the Query.

27. Select **Done Editing** for the Workbook.

28. Select **Save** and select **Save** again if prompted.

29. Select **Workbooks** in the Azure Sentinel portal.

30. Select the **My workbooks** tab.

31. Select the workbook you just created.

32. Select **View saved workbook**.

## You have completed the lab.
