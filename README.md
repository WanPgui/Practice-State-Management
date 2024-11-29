Option 1: State Management with Provider - Favorites Management App
Create a new Flutter project.
Add the Provider package:
Add provider: ^6.0.5 to your pubspec.yaml file and run flutter pub get.
Create a Favorites model:
In the lib directory, create a new file called favorites.dart.
Define a Favorites class that extends ChangeNotifier:
A List<String> named items to store favorite items.
Methods like addItem(String item) and removeItem(String item) to manage favorites.
Use notifyListeners() after modifying the list to update the UI.
Create a Product List UI:
In main.dart, wrap MaterialApp with ChangeNotifierProvider to provide the Favorites class to the widget tree.
Use a Scaffold with an AppBar titled "Product List".
Use ListView.builder inside the body of Scaffold to display a list of product items.
For each item:
Use a Card widget with Text to display product details.
Add an IconButton to add the product to favorites.
Favorites Screen:
Add a FloatingActionButton in the product list screen that navigates to the favorites screen.
Create a new screen to display favorite items using ListView.builder.
Wrap ListView.builder with a Consumer<Favorites> widget to update the list automatically when an item is added or removed.
Make It Interactive:
Allow users to remove items from favorites by adding an IconButton with a delete icon.
Test Your App:
Verify that users can add items to the favorites list and view or manage them on the favorites screen.
