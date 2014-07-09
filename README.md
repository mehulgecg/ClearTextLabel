# ClearTextLabel - iOS (Objective-C)

`ClearTextLabel` is a `UILabel` subclass that creates a label with see-through text.

## Requirements
* iOS 6.0 or later
* CoreText.Framework
* ARC (either project is ARC or ClearTextLabel is compiled with `-fobjc-arc`)

## How To Use

Using ClearTextLabel is as simple as using regular UILabel :

	ClearTextLabel* objCTLbl = [[ClearTextLabel alloc] initWithFrame:CGRectMake(20, 100, 280, 368)];
    objCTLbl.text = @"Can this be drawn with transparency ?";
    [self.view addSubview:objCTLbl];

ClearTextLabel draws the text provided to it with transparency.
* It uses CoreGraphics Context to draw the letters' CGPath.
* Letters' CGPath, how ? Well what's CoreText there for ?


## How It Looks
![Screenshot] (https://raw.githubusercontent.com/taruntyagi697/ClearTextLabel/master/Screenshot.png)

    
## Demo App
    Demo app includes the most basic regular example just for reference.