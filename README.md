# StripedTextTableViewController

A simple log viewer in Objective-C.

## Usage

```objective-c
StripedTextTableViewController *controller = [[StripedTextTableViewController alloc] initWithPath:aLogFilePath];
controller.allowTrash = NO;
controller.allowSearch = YES;
controller.tapToCopy = YES;
controller.rowSeparator = @"\r\n";
[aNavigationController pushViewController:controller animated:YES];
```
