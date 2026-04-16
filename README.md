# How to achieve default Enter/Escape behavior (IsDefault/IsCancel) with Syncfusion ButtonAdv in WPF

WPF’s standard Button supports default and cancel behavior via IsDefault and IsCancel, allowing Enter to invoke the default action and Escape to invoke the cancel action. Syncfusion’s ButtonAdv does not expose these properties directly. This sample demonstrates how to simulate the same behavior by handling the Window’s PreviewKeyDown event to invoke ButtonAdv click events for Enter and Escape.

## What this sample shows

* Simulate IsDefault (Enter) and IsCancel (Escape) for ButtonAdv
* Keep keyboard shortcuts consistent with standard WPF Button behavior
* A simple and non-invasive pattern that works alongside your existing UI
* Handle key input at the window level before focused controls process it
* Invoke the appropriate ButtonAdv action when the user presses Enter or Escape

This approach is useful for dialog-style windows and forms where keyboard accessibility and expected WPF interaction behavior are important.
