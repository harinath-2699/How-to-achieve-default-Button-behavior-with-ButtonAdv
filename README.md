# How to achieve default Button behavior with ButtonAdv
In WPF applications, the standard `Button` control provides built-in support for default and cancel button behaviors through the `IsDefault` and `IsCancel` properties. These properties allow a button to respond to the Enter and Escape keys respectively, enhancing user experience by enabling keyboard shortcuts for common actions. However, when using the `ButtonAdv` control from Syncfusion, these properties are not available by default.

To simulate this behavior with `ButtonAdv`, we can handle the `PreviewKeyDown` event of the `MainWindow`. Within this event handler, we can check if the Enter or Escape key was pressed and programmatically invoke the corresponding `ButtonAdv` click event. This approach effectively mimics the default and cancel behavior, allowing developers to maintain consistency in UI interaction even when using enhanced controls like `ButtonAdv`.

# About the sample
This sample demonstrates how to implement default button behavior using `ButtonAdv`. It includes a simple WPF window setup where the `PreviewKeyDown` event is used to detect key presses and trigger the appropriate button actions. This technique ensures that users can still rely on familiar keyboard shortcuts, even when using advanced UI components.
