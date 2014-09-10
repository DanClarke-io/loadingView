loadingView
===========
You can customise the text, and update it as your download updates (or as you finish a segment of your function).

The basic functions are:

```
+(void)OBTshowLoading:(UIView *)view withText:(NSString *)text;
+(void)OBTshowLoading:(UIView *)view;
+(void)OBThideLoading:(UIView *)view;
+(void)OBTupdatetext:(NSString *)text forView:(UIView *)view;
+(void)OBTupdatetext:(NSString *)text andWidth:(CGFloat)width andLines:(int)lines forView:(UIView *)view;
```


The UIView you supply would be your controlling view, such as self.view or self.navigationcontroller.view.

As you can see, you would call this by typing: 

```
[loadingView OBTshowLoading:self.view];
```


Optionally, you could specify the text (as default, it says "loading...") like so: 

```
[loadingView OBTshowLoading:self.view withText:@"My Text"];
```

Once you have finished whatever you were loading, you can then close the view, by typing: 

```
[loadingView OBThideLoading:self.view];
```

I am constantly updating (*I don't use this function as much as I used to, so the updating hasn't happened recently...*) this library to finetune how it works, and tinker with existing settings, I will attempt to update this page as I update it.

This markdown document was created using [Mou](http://mouapp.com/)