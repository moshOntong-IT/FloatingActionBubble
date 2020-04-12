# Floating Action Bubble 

A Flutter package to create a nice menu using a Floating Action Button.


![Showcase](https://imgur.com/IbinJsI.gif)

## Installation

Just add `floating_action_bubble` to your [pubspec.yml](https://flutter.io/using-packages/) file

```yml
dependencies:
  floating_action_bubble: 0.0.1
```

## Example

```dart
class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        body: Placeholder(),
        floatingActionButton: FabCircularMenu(
          children: <Widget>[
            IconButton(icon: Icon(Icons.home), onPressed: () {
              print('Home');
            }),
            IconButton(icon: Icon(Icons.favorite), onPressed: () {
              print('Favorite');
            })
          ]
        )
      )
    );
  }
}
```

You can check for a more complete example in the [example](https://github.com/Darshan0/floating_action_bubble/master/example) directory.

## Customize

You can customize the widget appareance using the following properties:

| Property  | Description | Default |
|----------|-------------|---------|
| alignment | Sets the widget alignment | `Alignment.bottomRight` |
| ringColor | Sets the ring color | `accentColor` |
| ringDiameter | Sets de ring diameter | `screenWidth * 1.25` (portrait) <br> `screenHeight * 1.25` (landscape) |
| ringWidth | Sets the ring width | `ringDiameter * 0.3` |
| fabSize | Sets the FAB size | `64.0` |
| fabElevation | Sets the elevation for the FAB | `8.0` |
| fabColor | Sets the FAB color | `primaryColor` |
| fabOpenColor | Sets the FAB color while the menu is open. This property takes precedence over `fabColor` | - |
| fabCloseColor | Sets the FAB color while the menu is closed. This property takes precedence over `fabColor` | - |
| fabOpenIcon | Sets the FAB icon while the menu is open | `Icon(Icons.menu)` |
| fabCloseIcon | Sets the FAB icon while the menu is closed | `Icon(Icons.close)` |
| fabMargin | Sets the widget margin | `EdgeInsets.all(16.0)` |
| animationDuration | Changes the animation duration | `Duration(milliseconds: 800)` |
| animationCurve | Allows you to modify de animation curve | `Curves.easeInOutCirc` |
| onDisplayChange | This callback is called every time the menu is opened or closed, passing the current state as a parameter. | - |



## Contributing

I will be very happy if you contribute to this project, please submit a PR 😁