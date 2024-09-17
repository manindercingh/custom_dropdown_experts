Custom Searchable Dropdown
Easily add a powerful and customizable searchable dropdown widget to your Flutter app!

This plugin lets you seamlessly integrate a dropdown menu with built-in search functionality, enhancing the user experience by making it easier to find and select items from a list.

Key Features:

Intuitive Search: Effortlessly find specific items in your dropdown list through real-time search as you type.
Highly Customizable: Tailor the look and feel of your dropdown to match your app's design with various styling options for labels, dropdown items, and even custom suffix icons.
Flexible Data Types: Works seamlessly with a variety of item types, making it adaptable to your specific data needs.
Simple Integration: Easily incorporate the Custom Searchable Dropdown into your Flutter app with minimal effort.
**Getting Started **

Install the Package: Add the following line to your pubspec.yaml file:
YAML
dependencies:
custom_searchable_dropdown: ^1.0.0
Use code with caution.

Import the Package: Import the package into your Dart file:
Dart
import 'package:custom_searchable_dropdown/custom_searchable_dropdown.dart';
Use code with caution.

**Usage Example **

Here's a quick demonstration of how to use the CustomSearchableDropdown in your app:

Dart
Container(
decoration: BoxDecoration(
borderRadius: BorderRadius.circular(6.0),
border: Border.all(color: Colors.black),
),
child: CustomSearchableDropDown(
items: widget.values ?? [], // List of items to display
label: title, // Label text for the dropdown
labelStyle: TextStyle(
fontSize: 16.0,
fontFamily: 'ProximaRegular',
color: Colors.black,
),
dropdownItemStyle: TextStyle(
fontSize: 16.0,
fontFamily: 'ProximaRegular',
color: Colors.black,
),
suffixIcon: SvgPicture.asset(
'assets/user_image/ic_up_down_arrow.svg',
width: 10,
height: 10,
),
dropDownMenuItems: widget.values?.map((item) => item).toList() ?? [],
onChanged: (value) {
if (value != null) {
widget.onChange(value);
title = value;
}
},
),
)
Use code with caution.

Explanation:

items: This list holds the items you want to display in the dropdown.
label: The text displayed as a label for the dropdown.
labelStyle: Customize the style of the label text.
dropdownItemStyle: Style each item within the dropdown list.
suffixIcon: Use a custom icon to visually indicate the dropdown functionality.
onChanged: This callback function gets triggered whenever an item is selected by the user.
**Additional Information **

For a more comprehensive understanding and exploration of the package's functionalities, we encourage you to visit the following resources:

Documentation: (Include the link to your documentation here)
Sample Project: (Include the link to your sample project repository here)
**Contributing **

We appreciate your interest in contributing! Feel free to open issues or submit pull requests on our GitHub repository.

**Support **

If you encounter any issues using this package, please don't hesitate to file them on our issue tracker on GitHub. The package authors will do their best to assist you swiftly.