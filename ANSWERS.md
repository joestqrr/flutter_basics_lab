# ANSWERS.md

**Name:** Radj P. Delarmente
**Student ID:** 241-00032

## 1. GitHub link

https://github.com/joestqrr/flutter_basics_lab

## 2. Last three build() lines (Activity 2)

```
build() called: 4 glasses
build() called: 5 glasses
build() called: 6 glasses
```

## 3. Observations

- **Activity 2:** When `_glasses++` was outside `setState()`, the screen did not change when I tapped +, because Flutter was not told to redraw.
- **Activity 3:** Without `Expanded`, the box became only as wide as its content, so the three boxes were not equal.
- **Activity 5:** Changing the radius from 8 to 20 made the Elevated button more rounded. The other buttons did not change.

## 4. Review questions

1. A StatelessWidget never changes after it is drawn (example: `ProfileCard`). A StatefulWidget has data that changes (example: `WaterTrackerPage`).
2. The widget class creates the State object. The State class keeps the changing data and has `build()`.
3. The screen did not update, because only `setState()` tells Flutter to redraw.
4. `build()` is called when the screen first loads and after every `setState()` (each tap).
5. The main axis is the direction children are laid out. A Row's main axis is horizontal and its cross axis is vertical. A Column is the opposite.
6. The box shrank to fit its content. `Expanded` makes a child fill the free space in a Row or Column and share it equally.
7. `GridView.builder` builds only the visible items and scrolls. A Column builds everything at once and overflows.
8. A Stack puts widgets on top of each other. `Positioned(top: 8, left: 8)` pins the badge to the card's top-left corner.
9. ThemeData styles the whole app (example: `elevatedButtonTheme`). A widget style affects only that widget (example: a `TextStyle` on one `Text`).
10. `_ThemeDemoAppState` holds `_isDark`. The switch calls `_setDark`, which uses `setState()`, and `MaterialApp` then gets the new `themeMode`.
