# How to load multiple SfDataGrids to a layout ?
In this article, we will show you how to load multiple [.Net Maui DataGrid's](https://www.syncfusion.com/maui-controls/maui-datagrid) to a layout.

## xaml
The code below demonstrates how to load multiple SfDataGrid's to a Grid layout.
```
<ContentPage.BindingContext>
    <local:EmployeeViewModel x:Name="viewModel" />
</ContentPage.BindingContext>

<Grid RowDefinitions="50,*,50,*,50,*"
      ColumnDefinitions="*">

    <Label Text="First Grid"
           HorizontalOptions="Center"
           FontAttributes="Bold"
           TextColor="Blue"
           Grid.Row="0"
           Grid.Column="0" />

    <!-- First DataGrid -->
    <syncfusion:SfDataGrid Grid.Row="1" 
                           Grid.Column="0"
                           ColumnWidthMode="Auto"
                           GridLinesVisibility="Both"
                           HeaderGridLinesVisibility="Both"
                           ItemsSource="{Binding Employees}" />

    <Label Text="Second Grid"
           HorizontalOptions="Center"
           FontAttributes="Bold"
           TextColor="Blue"
           Grid.Row="2"
           Grid.Column="0" />

    <!-- Second DataGrid -->
    <syncfusion:SfDataGrid Grid.Row="3" 
                           Grid.Column="0"
                           ColumnWidthMode="Auto"
                           GridLinesVisibility="Both"
                           HeaderGridLinesVisibility="Both"
                           ItemsSource="{Binding Employees}" />

    <Label Text="Third Grid"
           HorizontalOptions="Center"
           FontAttributes="Bold"
           TextColor="Blue"
           Grid.Row="4"
           Grid.Column="0" />

    <!-- Third DataGrid -->
    <syncfusion:SfDataGrid Grid.Row="5" 
                           Grid.Column="0"
                           ColumnWidthMode="Auto"
                           GridLinesVisibility="Both"
                           HeaderGridLinesVisibility="Both"
                           ItemsSource="{Binding Employees}" />
</Grid>
``` 

![multipleGrids.png](https://support.syncfusion.com/kb/agent/attachment/inline?token=eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjM0MzQ2Iiwib3JnaWQiOiIzIiwiaXNzIjoic3VwcG9ydC5zeW5jZnVzaW9uLmNvbSJ9.FVV6vlOOJXbLnGNMCzG5Vu4x8sH9oTGRwqdVA-ntEWM)

[View sample in GitHub](https://github.com/SyncfusionExamples/How-to-load-multiple-SfDataGrids-to-a-layout)

Take a moment to explore this [documentation](https://help.syncfusion.com/maui/datagrid/overview), where you can find more information about Syncfusion .NET MAUI DataGrid (SfDataGrid) with code examples. Please refer to this [link](https://www.syncfusion.com/maui-controls/maui-datagrid) to learn about the essential features of Syncfusion .NET MAUI DataGrid (SfDataGrid).
 
##### Conclusion
 
I hope you enjoyed learning about how to load multiple SfDataGrid's to a Grid layout.
 
You can refer to our [.NET MAUI DataGrid’s feature tour](https://www.syncfusion.com/maui-controls/maui-datagrid) page to learn about its other groundbreaking feature representations. You can also explore our [.NET MAUI DataGrid Documentation](https://help.syncfusion.com/maui/datagrid/getting-started) to understand how to present and manipulate data. 
For current customers, you can check out our .NET MAUI components on the [License and Downloads](https://www.syncfusion.com/sales/teamlicense) page. If you are new to Syncfusion, you can try our 30-day [free trial](https://www.syncfusion.com/downloads/maui) to explore our .NET MAUI DataGrid and other .NET MAUI components.
 
If you have any queries or require clarifications, please let us know in the comments below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [Direct-Trac](https://support.syncfusion.com/create) or [feedback portal](https://www.syncfusion.com/feedback/maui?control=sfdatagrid), or the feedback portal. We are always happy to assist you!