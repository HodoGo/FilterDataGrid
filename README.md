### Основан на функциях фильтрации, поиска и статистики заголовка столбца DataGrid, созданных в библиотеке Material Design XAML.
### Код не самый совершенный, он предназначен только для вашей справки и изучения.

#### Как использовать：
#### App.xml 

```C# 
<Application.Resources>
   <ResourceDictionary>
            <ResourceDictionary.MergedDictionaries>
                <materialDesign:BundledTheme
                    BaseTheme="Light"
                    PrimaryColor="Blue"
                    SecondaryColor="Lime" />
                <ResourceDictionary Source="pack://application:,,,/MaterialDesignThemes.Wpf;component/Themes/MaterialDesignTheme.Defaults.xaml" />
                <!--  Other merged dictionaries here  -->
                <ResourceDictionary Source="pack://application:,,,/FilterDataGrid;component/Themes/Generic.xaml" />
            </ResourceDictionary.MergedDictionaries>
            <!--  Other app resources here  -->
    </ResourceDictionary>
</Application.Resources>
``` 
#### View
 ```C#   
 <Window . . .
       xmlns:FD="clr-namespace:FilterDataGrid;assembly=FilterDataGrid"
    <Grid>
                <FD:FilterDataGrid
                    x:Name="DataGridControl1"
                    AutoGenerateColumns="True"
                    CanUserAddRows="False"
                    FilterLanguage="Russian"
                    FooterItems="{Binding footerList}"
                    GridLinesVisibility="All"
                    HeadersVisibility="All"
                    IsReadOnly="True"
                    ItemsSource="{Binding dvList, UpdateSourceTrigger=PropertyChanged}"
                    ShowRowsCount="True" />
    </Grid>
</Window>
```

![image](https://user-images.githubusercontent.com/62784658/235885521-db6fe5db-89d4-4f99-a823-4a5c2d476e78.png)


#### Контекстное меню после нажатия правой кнопки по заголовку столбца

![image](https://user-images.githubusercontent.com/62784658/235885961-32bb89f4-64e0-4133-857a-d0f26cc1da6f.png)

#### Поддержка глобального поиска（Ctrl+F）

![image](https://user-images.githubusercontent.com/62784658/235886930-abdd0273-ce5c-4bb7-b6d1-aaf320b79bed.png)

#### Поддержка следующих языков

![image](https://user-images.githubusercontent.com/73624088/225267641-91bd956f-8819-4e71-9395-4d0e134be6b8.png)


