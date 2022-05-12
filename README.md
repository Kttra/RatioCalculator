# Ratio Calculator
A ratio calculator/scaler made in C# using .NET 6. Additionally, this program can get the ratio of an image by drawing a rectangle over it. A ratio calculator takes two ratios and scales both sides so that their ratios are equal. Values will be rounded for better viewing. This program was primarily made to get lower ratios of pictures.

I found myself constantly looking at the width and height of pictures and then lowering their values to get a smaller ratio (for better viewing sizes in readme files), so I decided to make the process easier by creating this application that both calculates different ratios and gets the ratio without needing to download the image.

<p align="center">
<img src="https://user-images.githubusercontent.com/100814612/167768320-b06cd149-2462-45af-9203-c34ea3c9f24a.png"><img>
</p>

**Realtime Calculations**
-------------------------------------
When the realtime checkbox is checked (is checked by default), the program will update the ratios while getting input. This can be disabled by manually unchecking the checkbox or pressing enter in one of the textboxes. Realtime update will priortize based on the ratios updated. If the a and b fields are filled and c updated, d will be calculated. If a, b, and d are filled, c will be calculated. If b, c, and d are filled, a will be updated and so on.

For easier usage, pressing enter in any textbox will toggle realtime off and on. Like other programs, pressing tab will cycle through the boxes and buttons.

**Input Validation**
-------------------------------------
The textboxes are setup so that only digits can be typed in. This is achieved through keypress event handlers. However, this does not prevent random characters from being copied and pasted in. We do have a safety measure in place though with tryparse. The calculated textbox will end up being set to 0 if a non-number character is pasted in a textbox.

Normal types of ratios are generally smaller like the image below. When working with pictures and videos of different sizes, the scaling starts to become much larger making it tedious to calculate without a program or calculator at hand. This is the reason why this program was made.

<p align="center">
<img src="https://user-images.githubusercontent.com/100814612/163684610-1167edfe-125f-40f5-8839-48bc09d9a147.png"><img>
</p>

**Get Ratio Button**
-------------------------------------
A new exciting feature added to the program. This newly added feature will take a screenshot of your computer screen after hiding the main form. The new form that pops up will take up the entire screen while taking in the image of the taken screenshot. You can think of it almost like it's transparent, but there's an added bonus. We can draw on the screen. This means we can form a rectangle around an existing image on the screen and get its ratio without needing to go through the hassle of downloading an image and looking at its properties.

To use the new feature, press on the "Get Ratio" button. The main form will be hidden and you can start to draw your rectangle. If you want to cancel, press esc. The main form will reappear like normal. However, if you are satisfied with your selection, press any key on your keyboard. This will tell the program to update the first ratio to match the rectangle you drew.

https://user-images.githubusercontent.com/100814612/167955892-3b382738-52f7-4e30-a9a5-ee16ae54bf00.mp4

**Other Projects**
-------------------
Below are other similar projects related to this application that have helped me come up with the get ratio feature.

[Screenshot Form](https://github.com/Kttra/ScreenshotForm) - A screenshot program that showcases how to screenshot your pc screen, screenshot the form itself, screenshot the controls contained in a panel, and display an image on a picture box.

[Screenshot Webpage](https://github.com/Kttra/ScreenshotWebpage) - A screen capture application. This one is different in the sense that it screenshots an entire webpage.

[Mouse Position](https://github.com/Kttra/MousePosition) - A program that shows the coordinates of the mouse. This is a simple program, but can lead to powerful projects. In the ratio calculator program itself, I utilize the mouse position to draw the rectangle and calculate both the width and height of it.
