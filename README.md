![image](https://github.com/xhzengAIB/LearnEnglish/raw/master/Screenshots/XHImageViewer.gif)
XHImageViewer
=============
XHImageViewer is images viewer, zoom image

## How to use
Easy to drop into your project. You can add this feature to your own project, `XHImageViewer` is easy-to-use.   
```objc
#import "XHImageViewer.h"    

XHImageViewer *imageViewer = [[XHImageViewer alloc] init];
imageViewer.delegate = self;
[imageViewer showWithImageViews:_imageViews selectedView:imageView];

_imageViews is mutiple imageViews(subClass UIImageView or UIImageView)
imageView is user touch imageView to selectedImageView
```

Easy to use download web image form the open source.
```objc
#import "UIImageView+XHURLDownload.h"

UIImageView *imageView = [[UIImageView alloc] initWithFrame:CGRectMake(0, 0, 160, 200)]
[imageView setDefaultLoadingView];
[imageView loadWithURL:[NSURL URLWithString:@"http://www.pailixiu.com/IMG_1388.JPG"]];

multiple api to use：
- (void)loadWithURL:(NSURL *)url placeholer:(UIImage *)placeholerImage;
- (void)loadWithURL:(NSURL *)url placeholer:(UIImage *)placeholerImage showActivityIndicatorView:(BOOL)show;
- (void)loadWithURL:(NSURL *)url placeholer:(UIImage *)placeholerImage showActivityIndicatorView:(BOOL)show completionBlock:(void(^)(UIImage *image, NSURL *url, NSError *error))handler;
```

## Profile

[CocosPods](http://cocosPods.org) is the recommended methods of installation XHImageViewer, just add the following line to `Profile`:

```
pod 'XHImageViewer'
```

## Lincense ##

`XHImageViewer` is available under the MIT license. See the LICENSE file for more info.
