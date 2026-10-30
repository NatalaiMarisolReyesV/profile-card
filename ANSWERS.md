# Answers

## 1. Default value of flexDirection in React Native
In React Native the default value of flexDirection is column, so the
elements are placed vertically, from top to bottom. On the web with CSS
the default is row, so the elements are placed horizontally.

## 2. justifyContent vs alignItems
justifyContent distributes and aligns the elements along the main axis
of the container. alignItems aligns them along the cross axis, which is
perpendicular to the main axis.

## 3. What flex: 1 does
Inside a row, flex: 1 makes the element expand horizontally to fill the
remaining space available between its siblings. On the outermost View of
a screen, it makes the View take up the whole screen.

## 4. resizeMode cover vs contain
With resizeMode="cover" the image is scaled keeping its proportions
until it completely fills the container, so parts of it may be cropped.
With resizeMode="contain" the whole image is shown inside the container,
keeping its proportions, but there may be empty space around it.

## 5. Why StyleSheet.create
StyleSheet.create keeps all the styles organized in one place and
validates them, instead of creating new plain objects inside the JSX on
every render. It also helps performance because the styles are defined
once and reused.

## 6. Why shadowColor doesn't work on Android
The standard shadow properties (shadowColor, shadowOffset, shadowOpacity
and shadowRadius) use the iOS shadow API, so they have no effect on
their own on Android. On Android the shadow is created with the
elevation property.