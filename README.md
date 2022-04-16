# RatioCalculator
A simple ratio calculator/scaler made in C# using .net 5.

The purpose of this program is to simulate a ratio calculator. A ratio calculator takes two ratios and scales both sides so that their ratios are equal. Values will be rounded for better viewing. This program was primarily made for scaling pictures.


<p align="center">
<img src="https://user-images.githubusercontent.com/100814612/163684311-a792f4db-77cd-4366-bf72-1523b795290e.png"><img>
</p>

**Realtime Calculations**
-------------------------------------
When the realtime checkbox is checked (is checked by default), the program will update the ratios while getting input. This can be disabled by manually unchecking the checkbox or pressing enter in one of the textboxes. Realtime update will priortize based on the ratios updated. If the a and b fields are filled and c updated, d will be calculated. If a, b, and d are filled, c will be calculated. If b, c, and d are filled, a will be updated and so on.

**Input Validation**
-------------------------------------
The textboxes are setup so that only digits can be typed in. This is achieved through keypress event handlers. However, this does not prevent random characters from being copied and pasted in. We do have a safety measure in place though with tryparse. The calculated textbox will end up being set to 0 if a non-number character is pasted in a textbox.



