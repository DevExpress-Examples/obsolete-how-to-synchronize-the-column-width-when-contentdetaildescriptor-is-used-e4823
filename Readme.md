<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128653373/13.1.5%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/E4823)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
[![](https://img.shields.io/badge/💬_Leave_Feedback-feecdd?style=flat-square)](#does-this-example-address-your-development-requirementsobjectives)
<!-- default badges end -->
<!-- default file list -->
*Files to look at*:

* [DetailSyncBehavior.cs](./CS/DXGrid.ColumnSync/DetailSyncBehavior.cs) (VB: [DetailSyncBehavior.vb](./VB/vb_DXGrid.ColumnSync/DetailSyncBehavior.vb))
* [MainWindow.xaml](./CS/DXGrid.ColumnSync/MainWindow.xaml) (VB: [MainWindow.xaml](./VB/vb_DXGrid.ColumnSync/MainWindow.xaml))
* [MainWindow.xaml.cs](./CS/DXGrid.ColumnSync/MainWindow.xaml.cs) (VB: [MainWindow.xaml.vb](./VB/vb_DXGrid.ColumnSync/MainWindow.xaml.vb))
* [ViewModel.cs](./CS/DXGrid.ColumnSync/ViewModel.cs) (VB: [ViewModel.vb](./VB/vb_DXGrid.ColumnSync/ViewModel.vb))
<!-- default file list end -->
# How to synchronize the column width when ContentDetailDescriptor is used


<p>This example demonstrates how to implement column width synchronization in Master-Detail DXGrid mode with ContentDetailDescriptor.</p>
<p>In this example, we have created a DetailSyncBehavior class that performs synchronization between Master Grid columns and Detail Grid columns, in accordance with the visible indexes of columns.</p>
<p>This class can easily be attached to the <strong>Detail</strong> GridControl object in the following manner:</p>


```xaml
           <dxg:ContentDetailDescriptor>
                    <dxg:ContentDetailDescriptor.ContentTemplate>
                        <DataTemplate>
                            <dxg:GridControl ItemsSource="{Binding Details}" AutoGenerateColumns="AddNew" MaxHeight="150">
                                <i:Interaction.Behaviors>
                                    <local:DetailSyncBehavior />
                                </i:Interaction.Behaviors>
                                <dxg:GridControl.View>
                                    <dxg:TableView ShowGroupPanel="False"/>
                                </dxg:GridControl.View>
                            </dxg:GridControl>
                        </DataTemplate>
                    </dxg:ContentDetailDescriptor.ContentTemplate>
                </dxg:ContentDetailDescriptor>
```


<p> </p>

<br/>


<!-- feedback -->
## Does this example address your development requirements/objectives?

[<img src="https://www.devexpress.com/support/examples/i/yes-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=how-to-synchronize-the-column-width-when-contentdetaildescriptor-is-used-e4823&~~~was_helpful=yes) [<img src="https://www.devexpress.com/support/examples/i/no-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=how-to-synchronize-the-column-width-when-contentdetaildescriptor-is-used-e4823&~~~was_helpful=no)

(you will be redirected to DevExpress.com to submit your response)
<!-- feedback end -->
