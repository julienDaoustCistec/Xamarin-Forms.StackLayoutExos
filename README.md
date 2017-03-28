# Xamarin-Forms.StackLayoutExos

 StackLayout
By: Mosh Hamedani
Exercise 1
  1
• • •
•
•
Page background color: #127ac7 Buttons background color: #1dabf0 Welcome label properties:
• FontSize=“30”
• FontAttributes=“Bold”
• HorizontalOptions=“Center”
Cross-platform label properties: • FontSize = “18”
Tip: Note that the buttons are stretching horizontally to fill the page. This suggest that HorizontalOptions property of StackLayout is Fill (default). On the other side, all the elements are vertically in the center. So, you should set VerticalOptions property of the StackLayout to center.
 StackLayout
By: Mosh Hamedani
Exercise 2
This design is similar to Instagram app. You can see that a few elements are stacked vertically (username, image, buttons, a horizontal line, number of likes, etc).
Padding
Note that the image is filling the entire page horizontally, but we have some padding around other elements. To implement this, you can have a parent StackLayout that fills the page horizontally, and a nested StackLayout with some padding.
Image
Use an Image with Source=“http://
lorempixel.com/1920/1080/nature/3/“
Horizontal Line
To draw a horizontal line above “700
likes”, use a BoxView with
Color=#f0f0f0 and HeightRequest=1.
In Xamarin, we cannot explicitly set the
height or width of elements. Instead, we use HeightRequest or WidthRequest. We request a given height/width and the runtime decides the actual height/width. That’s why Height and Width properties are read-only.
Padding for iOS
Finally, make sure to apply 20 units padding on top of the page for iOS only. Use OnPlatform for that.
    2
