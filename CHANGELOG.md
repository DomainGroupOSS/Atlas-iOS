# LayerUIKit Change Log

## x.x.x

### Public API Changes

* `-[LYRUIAddressBarControllerDataSource searchForParticipantsMatchingText:completion:]` is now `-[LYRUIAddressBarControllerDataSource addressBarViewController:searchForParticipantsMatchingText:completion:]`. That is, the view controller is now passed as the first parameter. This callback also now controls the order of search results by providing an `NSArray` instead of an `NSSet` in the completion block.
* The `maxHeight` property of `LYRUIMessageComposeTextView` has been removed. Use the `maxNumberOfLines` property of `LYRUIMessageInputToolbar` instead.
* `-[LYRUIMessageComposeTextView insertImage:]` has been removed. Use `-[LYRUIMessageInputToolbar insertImage:]` instead.
* `-[LYRUIMessageComposeTextView removeAttachements]` has been removed. It doesn't have a replacement since it was meant for internal use only.
* The `placeHolderText` property of `LYRUIMessageComposeTextView` is now `placeholder`.