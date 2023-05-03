Основан на функциях фильтрации, поиска и статистики заголовка столбца DataGrid, созданных в библиотеке Material Design XAML.
Код не самый совершенный, он предназначен только для вашей справки и изучения.

Как использовать：App.xml ResourceDictionary

  
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
   
   
 <Window . . .
       xmlns:FD="clr-namespace:FilterDataGrid;assembly=FilterDataGrid"
    <Grid>
 
    </Grid>
</Window>

![image](https://user-images.githubusercontent.com/73624088/225265390-f9e90483-5a6e-402e-828a-fa8117407791.png)

Контекстное меню после нажатия правой кнопки по заголовку столбца

![image](https://user-images.githubusercontent.com/73624088/225265847-f24406f9-ef58-4990-88dc-c9d0ba52705e.png)

Поддержка глобального поиска（Ctrl+F）

![image](https://user-images.githubusercontent.com/73624088/225266292-50c16732-48f5-4962-8233-56a334071589.png)

Поддержка следующих языков

![image](https://user-images.githubusercontent.com/73624088/225267641-91bd956f-8819-4e71-9395-4d0e134be6b8.png)


