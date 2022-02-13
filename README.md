# StripedTextTableViewController

A simple log viewer in Objective-C.

## Usage

```objective-c
StripedTextTableViewController *ctrl = [[StripedTextTableViewController alloc] initWithPath:[[NSBundle mainBundle] pathForResource:@"keybagd.log" ofType:@"0"]];
ctrl.reversed = YES;
ctrl.allowTrash = NO;
ctrl.allowSearch = YES;
ctrl.pullToReload = YES;
ctrl.tapToCopy = YES;
ctrl.pressToCopy = YES;
ctrl.preserveEmptyLines = NO;
ctrl.removeDuplicates = YES;
ctrl.rowSeparator = @"\n";
ctrl.rowPrefixRegularExpression = [NSRegularExpression regularExpressionWithPattern:@"^(Mon|Tue|Wen|Thu|Fri|Sat|Sun)\\s" options:kNilOptions error:nil];
UINavigationController *navCtrl = [[UINavigationController alloc] initWithRootViewController:ctrl];
[self presentViewController:navCtrl animated:YES completion:nil];
```
