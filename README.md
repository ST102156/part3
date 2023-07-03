
# part3
Window x:Class="WpfApp1.ScaleQue"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
        xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
        xmlns:local="clr-namespace:WpfApp1"
        mc:Ignorable="d"
Title="Recipe" Height="600" Width="800">
    <Grid Margin="20,20,25,29">
        <Grid.RowDefinitions>
            <RowDefinition Height="Auto"/>
            <RowDefinition Height="Auto" MinHeight="114"/>
            <RowDefinition/>
        </Grid.RowDefinitions>

        <!-- Add Recipe Section -->
        <Border Background="Fuchsia" Padding="10" Margin="0,0,-15,20">
            <TextBlock Text="Add Recipe" FontSize="30" FontWeight="DemiBold" HorizontalAlignment="right" Foreground="GhostWhite"/>
        </Border>

        <Grid Grid.Row="1" Background="Pink" Margin="0,0,-15,20">
            <Grid.ColumnDefinitions>
                <ColumnDefinition Width="Auto"/>
                <ColumnDefinition/>
                <ColumnDefinition Width="Auto"/>
            </Grid.ColumnDefinitions>

            <StackPanel Grid.Column="0" VerticalAlignment="Top" Margin="0,10">
                <TextBlock Text="Recipe Name:" FontWeight="Bold" Foreground="White"/>
                <TextBox x:Name="RecipeNameTextBox" Background="LightYellow" Width="300" Margin="0,5"/>
            </StackPanel>
