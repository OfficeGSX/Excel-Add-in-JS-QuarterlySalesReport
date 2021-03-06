# Quarterly Sales Report Task Pane Add-in Sample for Excel 2016

_Applies to: Excel 2016_

This is a simple Excel task pane add-in that loads some data into a worksheet and creates a basic chart in Excel 2016. It comes in two flavors: code editor and Visual Studio.

![Quarterly Sales Report Sample](images/QuarterlySalesReport_report.PNG)

## Try it out
### Code editor version

The simplest way to deploy and test your add-in is to copy the files to a network share.

1.  Deploy the source files in the Code Editor Proj folder by using your favorite server.
2.  Open the manifest file (QuarterlySalesReportManifest.xml) and replace https://yourserver with the name of your server. (i.e. https://localhost) You will do this in both the \<SourceLocation\> element and the \<Urls\> element.
3.  Copy the manifest (QuarterlySalesReportManifest.xml) to a network share (for example, \\\MyShare\MyManifests).
4.  Add the share location that contains the manifest as a trusted app catalog in Excel.

    a.  Launch Excel and open a blank spreadsheet.

    b.  Choose the **File** tab, and then choose **Options**.

    c.  Choose **Trust Center**, and then choose the **Trust Center Settings** button.

    d.  Choose **Trusted Add-ins Catalogs**.

    e.  In the **Catalog Url** box, enter the path to the network share you created in step 3, and then choose **Add Catalog**.

   f.  Select the **Show in Menu** check box, and then choose **OK**. A message appears to inform you that your settings will be applied the next time you start Office.

5.  Test and run the add-in.

    a.  In the **Insert tab** in Excel 2016, choose **My Add-ins**.

    b.  In the **Office Add-ins** dialog box, choose **Shared Folder**.

    c.  Choose **Quarterly Sales Report Sample**>**Insert**. The add-in opens in a task pane to the right of the current worksheet, as shown in the following figure.

  ![Quarterly Sales Report Sample](images/QuarterlySalesReport_taskpane.PNG))

    d.  Click the **Click me!** button to render the data and the chart inside the worksheet, as shown in the following figure.  To see the chart update dynamically, just change the data in the range.

  ![Quarterly Sales Report Sample](images/QuarterlySalesReport_report.PNG)

### Visual Studio version
1.  Copy the project to a local folder and open the Excel-Add-in-JS-QuarterlySalesReport.sln in Visual Studio.
2.  Press F5 to build and deploy the sample add-in. Excel launches and the add-in opens in a task pane to the right of a blank worksheet, as shown in the following figure.

  ![Quarterly Sales Report Sample](images/QuarterlySalesReport_taskpane.PNG)

3. Click the **Click me!** button to render the data and the chart inside the worksheet, as shown in the following figure.  To see the chart update dynamically, just change the data in the range.

  ![Quarterly Sales Report Sample](images/QuarterlySalesReport_report.PNG)

## Code it

If you want to write this add-in yourself from scratch, see [Build your first Excel Add-in](https://github.com/OfficeDev/office-js-docs/blob/master/excel/build-your-first-excel-add-in.md).


### Learn more


1.  [Excel Add-ins programming overview](https://github.com/OfficeDev/office-js-docs/blob/master/excel/excel-add-ins-programming-overview.md)
2.  [Snippet Explorer for Excel](http://officesnippetexplorer.azurewebsites.net/#/snippets/excel)
3.  [Excel Add-ins code samples](https://github.com/OfficeDev/office-js-docs/blob/master/excel/excel-add-ins-code-samples.md)
4.  [Excel Add-ins JavaScript API Reference](https://github.com/OfficeDev/office-js-docs/blob/master/excel/excel-add-ins-javascript-reference.md)
5.  [Build your first Excel Add-in](https://github.com/OfficeDev/office-js-docs/blob/master/excel/build-your-first-excel-add-in.md)