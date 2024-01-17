# Figma: Planet Burgers order form

## setup

1. create a page called assets
2. create a page called design system
3. creat a page called components
4. create a page called mobile

## Import Assets

3. import header image
4. with proportions constrained, make it 390px wide
5. make a component with header image called _img/bg/header_
6. import footer image
7. with proportions constrained, make it 390px wide
8. make a component with the footer image called _img/bg/footer_
9. import logo
10. with logo selected, in selection colours, make styles _img/logo/primary_, _img/logo/secondary_, _img/logo/accent_.
11. import star image
12. with required selected, make a component called _img/star_
13. import required icon
14. with required selected, make a component called _img/icon/required_
15. 9. import logo
16. with required selected, make a component called _img/logo_

## set up colour styles

16. with logo selected, in selection colours, make styles _img/logo/primary_, _img/logo/secondary_, _img/logo/accent_.
17. sample dark blue on header image and make a colour style called _body/bg_

## create footer and header components

18. place an instance of assets/img/bg/footer on the canvas
19. open the _planet-burger-text.txt_ file and copy the contact info
20. paste the contact info over the footer instance
21. apply text style _body/p_ and center it
22. select the text and image and align center
23. with the selection, create a new component called _webparts/footer_
24. place an instance of assets/img/bg/header on the canvas
25. place an instance of assets/img/logo on the canvas
26. vertically and horizontally align the logo and background
27. select them both and make a new component called _webparts/header_

## set up typography

28. change to page _design system_
29. Type the words _body/p_
30. make a text style called _body/p_
31. Type the words _body/h1_
32. make a text style called _body/h1_
33. Type the words _body/h2_
34. make a text style called _body/h2_
35. Type the words _form/label_
36. make a text style called _form/label_
37. Type the words _form/element-label_
38. make a text style called _form/element-label_

## Make a form label that can be required or not

39. type text _form label_
40. Apply the style _form/label_ to the text _form label_
41. duplicate _form label_
42. drag an instance of _required_ image and position beside the second _form label_
43. drag around _form label_ and _required_
44. select _auto layout_ from the properties panel
45. select both _form label_ instances and make into a component set
46. name the component _form/label_
47. in the properties panel, in the variant section, change _property 1_ to _required_.
48. in the component, select the first _form label_ and in the properties panel change _form label_ to _no_
49. in the component, select the second _form label_ (with the asterisk) and in the properties panel change _frame 1_ to _yes_
50. **TEST** drag an instance of _form/label_ from the assets panel
51. **TEST** in the properties, toggle _required_ to see what happens
52. **TEST** with _form/label_ in _required_ mode, double click the text and change the label. The asterisk should accommodate the change in test length (this is the auto layout in action)

## Make a checkbox

53. with the rectangle tool, make a 20px X 20px square, 1px black border, white fill, 2px border radius
54. duplicate the square
55. make another square, 14px X 14px, no border, black fill, 2px border radius and align it horizontal/vertical with the square you made in step 53.
56. Group together the outer and inner checkbox you jus created
57. in the property sidebar, change _property 1_ to _selected_
58. in the property sidebar, change _group 1_ to _yes_
59. in the property sidebar, change _Rectangle 1_ to _no_
60. select the component and rename to _form/input/checkbox-static_

## Make a selectable checkbox

61. Duplicate the checkbox component you created in step 60.  
    **_IMPORTANT:_** _make sure you are duplicating the original component, not placing an instance_
62. rename it to _form/input/checkbox-auto_
63. With _form/input/checkbox-auto_ component selected, open the prototype panel on the right
64. drag a wire from _Rectangle 1_ to _Group 1_, make sure properties are **on tap** and **change to**
65. drag a wire from _Group 1_ to _Rectangle 1_, make sure properties are **on tap** and **change to**

## Make a button

66. make a 100px X 60px rectangle
67. apply the logo>secondary colour for the fill
68. apply a 15px border radius
69. select the box then select the text tool
70. Add text _Button_, make it white, centered and 18px
71. vertical/horizontal align the text and the box using the properties panel
72. select text and box and apply auto layout from the properties panel
73. turn the box/text into a component and call it _form/input/button_

## create the first page

74. go to page _mobile_
75. Add a new frame and call it _order form_
76. Add a frame and select _iPhone 14_ from the presets
77. rename the frame to _home 000_ The numbers are a naming convention that will help us identify the states of the form
78. with the frame selected, apply the color _body/bg_
79. from the assets panel, drag the header component and footer component.
80. Select the frame by clicking on its title. Use the eyedropper in the fill panel to select the dark color from the header image.

## Add page title

81. Add the title Text is _body/h1_, align center, make it white

## make the form

82. add _form/label_ component, change text colour to white, add text “choose a topping” and position on the frame, in properties, use the required variant.
83. add three _form/checkbox-static_ components, align in a column and place a topping beside each checkbox and use the _form/item-label_ text style
84. add a _form/checkbox-auto_ component and place under the order form. Add text beside for people to sign up to the mail list. Again, use white _form/item-label_
85. add a button component, change the text to “Order” and center the button.
86. Align everything so it looks right to you.
87. Using the same steps you did for the header and footer, turn the entire form into a component and move it to the _Local components_ page
88. use the play button check your work

## Creating frames for selections

Since users are required to select a topping, we cannot use our auto-checkbox. We need some way of controlling what they are doing. We will do this by making a new frame for each potential state of the order form. A checkbox can be on or off, so we need to know all the states ahead of time. It helps to have a naming convention to do this. So with 0 being off, and 1 being on, our possibilities are:

<table style="border: 1px solid black; padding: 1em;">

<thead>
<tr>
<th style="text-align: center; width: 33.33%;">anchovies</th>
<th style="text-align: center; width: 33.33%;">onions</th>
<th style="text-align: center; width: 33.33%;">mushrooms</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center; width: 33.33%;">0</td>
<td style="text-align: center; width: 33.33%;">0</td>
<td style="text-align: center; width: 33.33%;">0</td>
</tr>
<tr>
<td style="text-align: center; width: 33.33%;">1</td>
<td style="text-align: center; width: 33.33%;">0</td>
<td style="text-align: center; width: 33.33%;">0</td>
</tr>
<tr>
<td style="text-align: center; width: 33.33%;">1</td>
<td style="text-align: center; width: 33.33%;">1</td>
<td style="text-align: center; width: 33.33%;">0</td>
</tr>
<tr>
<td style="text-align: center; width: 33.33%;">1</td>
<td style="text-align: center; width: 33.33%;">0</td>
<td style="text-align: center; width: 33.33%;">1</td>
</tr>
<tr>
<td style="text-align: center; width: 33.33%;">1</td>
<td style="text-align: center; width: 33.33%;">1</td>
<td style="text-align: center; width: 33.33%;">1</td>
</tr>
<tr>
<td style="text-align: center; width: 33.33%;">0</td>
<td style="text-align: center; width: 33.33%;">1</td>
<td style="text-align: center; width: 33.33%;">0</td>
</tr>
<tr>
<td style="text-align: center; width: 33.33%;">0</td>
<td style="text-align: center; width: 33.33%;">1</td>
<td style="text-align: center; width: 33.33%;">1</td>
</tr>
<tr>
<td style="text-align: center; width: 33.33%;">0</td>
<td style="text-align: center; width: 33.33%;">0</td>
<td style="text-align: center; width: 33.33%;">1</td>
</tr>
</tbody>
</table>

1. make seven copies of frame _home 000_, name each one _100_, _101_ etc. You do not need option 000 because that’s where we start (home).
2. click on your order form component until you have selected the checkbox inside it. In the properties panel, turn on check boxes so they match the name of the frame. For example, anchovies, onions but no mushrooms would be 110. (on, on, off)

## Create frames for confirmation and required

91. make two more copies of _home 000_, we will use these later. For now, call name the frames _confirmation_ and _required_

## Connect all the options

**Don’t do all of these unless there is time**

92. start with _home 000_ , select the prototype panel and wire each option to its destination. (on tap - navigate to - destination). For example, if I’m on _home 000_ and I select the second option, I go to _option 010_ (the second option is on), if I’m on _option 111_ (everything selected) and I click the last option, I’ll go to _option 101_ because I’ve deselected the second option.
93. Test. If you did it right, when you hit play you will select and deselect smoothly.

## Make a required page and wire it to corresponding frames

94. go to frame _required_ and open the design panel.
95. Add text “Toppings are required”
96. draw a red box around the toppings list to draw attention to it. (draw a box, no fill, border 2px red)
97. for each option in the toppings check boxes, go to the prototype panel and wire it to the corresponding frame, see step 86 for details.

## make the confirmation page

98. go to frame _Confirmation_
99. remove the order form instance.
100.  copy the confirmation text from planet-burgers-text.txt
101.  select the text tool and draw a box in the frame, this will give you a resizable text field. Paste the copied text and apply a white _body/p_ style and position, so it looks decent.
102.  drag a few instances of the star component to the frame

## finishing up

103. on frame _home 000_ wire the order button to frame _required_,
104. on frame _Confirmation_ wire the logo to _home 000_
105. on all remaining frames, wire the order button to _Confirmation_ frame
