Download Link: https://assignmentchef.com/product/solved-rental-calculator-for-the-skyforest-apartments
<br>
You are to develop a rental calculator for the Skyforest Apartments, a lushly landscaped mega-complex located at the base of the mountains. The mega-complex is divided into three areas: Northern Lights, Rocky Terrace, and Chinook Village, each of which has their own unique character and quality of units. The rental calculator allows the user to enter a base rent (which would be the minimum rent charged for a standard version of the least expensive unit type) and then to select a variety of attributes about an apartment, include:

* number of bedrooms* number of bathrooms* view* location* amenities, including fireplace, extra parking space, non-smoking buildingThe combination of attributes determines the ultimate monthly rent to be paid. Moreover, the program figures out the deposit amount too, based on type of pet, credit rating of the renter, and other factors.

The attributes are to be selected, and then upon pressing of an on-screen Calculate Rent button, the rent and deposit are calculated and displayed.

You are to develop this program using Visual Basic.




Functional Specifications

An executable sample version of the program (.exe file only) is downloadable from the main screen for this assignment. This sample version shows the basic user interface you should use. Although the sample program itself is reasonably accurate, it has not been fully tested and the rent and deposit amounts shown may be incorrect in certain instances other than with the grading criteria data. The access keys are, though, fully represented in this interface. Please use the functional specifications below to determine actual function, unless otherwise noted. Please do note, however, that the dynamic enabling and disabling of controls based on values selected does work properly in the sample; your program should perform the same way.

A static picture of the form is available. Please view it if you are having trouble running the sample program

You are to develop a form laid out just like the one in the sample version, complete with the same controls. Control locations and control/form sizes should be approximately the same. Access keys for the Base Rent, Area, Calculate button, Exit button and menu (menu title and menu items) should also be the same as with the sample version. Keep in mind that for access keys to work properly, you should establish a proper tab order that places the base rent text box immediately after its label (and similar for the Area combo box and its label). These are the only two requirements for tab order, however, the rest of the form’s tab order should be established in a decent logical way.

The program’s executable build uses the standard “XP Look”, so the program should appear the same on Windows XP, Vista, 7 and 8.x, and the various versions of VB. However, in case of a slight shift due to a newer version of VB, there’s no reason to panic or contort the look of any of the controls; the program basically uses the “natural” look of each control.

Each of the items in the chart (except area) adds onto either base rent, deposit or both. Selection of some options excludes the availability of other options, and these will be noted below. The area specifies a multiplier to a standard rent charge, based on which area is selected. Standard rent is defined as the base rent plus all the options selected.

You will note several group boxes. Please be aware of the instructions below for creating option groups, as each group is exclusive of the others.

The base rent can be any number from 500 up. If it is less than 500, a Critical-style message box should be displayed indicating the error. The error text should read: Base rent must be 500 or higher, the box title should say Input Error and the button should be OK. If the rent is non-numeric, a Critical-style message box should be displayed indicating the error. The error text should read: Base rent must be a number, the box title should say Input Error and the button should be OK. Design your program so that it uses a defined constant for the minimum possible base rent, as well as for the initial base rent.

Area is a dropdown list style of combo box that has one of the areas specified above:

· Northern Lights is the standard area.

· Rocky Terrace units are more luxurious and add a premium of 40% to the standard rent after calculating for all options.

· Chinook Village is quaint and high demand, although the units are smaller, and adds a premium of 10% to the standard rent after calculating for all options. There are no Mountain Foliage views in Chinook Village, so selection of Chinook Village should disable that view. (Remember to re-enable the view for other areas.) If Mountain Foliage is the view already selected and the user selects Chinook Village, the view should change to Courtyard.

For bedrooms, single units are covered by the base rent. One bedroom units are $200 higher than base. One and den units are $325 higher than base. Two bedroom units are $400 higher than base. Single units never have more than one full bathroom, so selection of Single should disable the other bathroom options. One bedroom units and one and den units never have two full bathrooms, so selection of either should disable two full baths. Two bedroom units never have only one bathroom; they always have one and a half baths or two baths, so disable one bath if two bedroom is selected. Remember always to re-enable the options for other size units.

For one bedroom units and one and den units, having one and a half baths is a $50 premium over the standard one bath. For two bedroom units, having two baths is a $35 premium over the standard one and a half baths.

For views, courtyard is standard. Parking lot views (called “automotive” on the form) give a discount of $10 off the rent. Mountain foliage views–if available–command a premium of $62. Creek and waterfall views are especially prized and command a premium of $101.

Fireplaces are plentiful throughout the complex, so not having one is rare and would constitute a $15 per month discount. This item should already be “checked” upon entering the form.

Some of the units are on non-smoking floors or buildings, and these are prized by many prospective renters. There is a $10 per month premium on these.

Each extra parking space is $35 per month, and is subject to availability. Parking is NOT part of the standard rent (therefore not subject to area multipliers) and is the same price in all areas of the mega-complex. It should, though, be included in the on-screen rent display and it does figure into the deposit.

Having a storage facility available is an extra bonus enjoyed by Skyforest residents. To use the storage facility, you must pay an additional $90 per month (plus additional deposit–see below). Storage is part of the standard rent (subject to area multipliers). Like other standard rent options, it should be included in the on-screen rent display and also figures into the deposit.

The deposit is generally equal to one month’s final rent (after applying all options and multipliers to the standard rent, plus parking). However, if the renter has a dog, the deposit is $75 higher. If a cat, the deposit is $125 higher. Having a storage facility in any section of the complex adds $42 to the deposit. And for renters with bad credit, the entire deposit (including premiums, and after rounding) is doubled.




Other Specifications

Both rent and deposit boxes have 3D “sunken” look (and the user should not be able to tab or click into them), so be sure to pick the right control and properties for this. Try your best to match the colors; their names are Aqua and Yellow. The labels for them should be bold and large as shown. The amounts inside both should be bold and large as shown, and should show a $ in front of the number. Optionally, the number may be formatted with a comma for numbers over 999 (not a requirement). The final rent amount and deposit amount should not have any decimal points or decimal values and should be rounded to the nearest integer value. (How do you round in Visual Basic? You get to look up this function!) Both boxes should be completely empty upon program start. If either of the error conditions described above occur (base rent less than 500 or base rent being non-numeric), both the rent and deposit box should display the word Error upon the user clicking the Calculate Rent button and the appropriate Input Error message box should then pop up on-screen. Once the user clears the message box, Errorshould still display in the rent and deposit boxes.

The base rent box should contain the minimum possible base rent (see above) upon starting the program. The default area which should be displayed is Northern Lights. The default bedroom size is one. The default bath is one. The default view is Courtyard. The default pets is Other Small or None. All the checkboxes should be unchecked except for Fireplace. Anything not available to one bedroom units should be disabled upon start of the program (to be re-enabled later if the appropriate option is selected).

When changing from one bedroom specification to another, if certain bath sizes (or other such attribute) are not available to the new specification, then those that are not must be disabled. Moreover, the default bath size (or other such attribute) should be automatically selected at that time.

“Disabling” a radio button does NOT mean making it invisible. It should only be grayed out (typically, by setting the Enable property to false).

Note that the form itself should have the title Skyforest Rental Calculator appearing in the title bar. Also, you should definitely include the other labels you see, including the name of the complex and its slogan.

The Exit button should end the program. The Calculate Rent button always needs to be pressed to determine the latest rent and deposit. Both of these use access keys; see the interface for more information.

It is possible for the final rent to be BELOW the base rent. For instance, selection of the least expensive unit that also has either an “automotive” view or no fireplace would do this, due to the fact that these items are discounts from the rent.

And Even More Specifications!

Your Skyforest program should incorporate a simple Windows menu. The menu title should be “Apartments” with the “r” underlined as the access key. (Remember, users typically will NOT see the underscore during execution until they press ALT.) The items on the menu should be: Featured Single, Featured 1-Bedroom, Featured 2-Bedroom, and Exit. The “S” is the access key in “Featured Single”. The “1” is the access key in “Featured 1-Bedroom”. The “2” is the access in “Featured 2-Bedroom”. The “x” is the access key in Exit.

Place one of those thin menu separator lines separating the three featured scenarios from the Exit menu item.

Selecting Featured Single sets the following on the form: single unit in Northern Lights, one full bath, courtyard view, no pets, fireplace checked. Other options should be unchecked.

Selecting Featured 1-Bedroom sets the following on the form: one-bedroom unit in Northern Lights, one full bath, automotive view, no pets, fireplace checked. Other options should be unchecked.

Selecting Featured 2-Bedroom sets the following on the form: two-bedroom unit in Northern Lights, one-and-a-half bath, automotive view, no pets, fireplace checked. Other options should be unchecked.

Pay close attention to all access keys on the form. Define only those access keys specified in the sample interface.

Clarifications

Again, it is possible to have the calculated rent be BELOW the base rent under certain circumstances. For instance, not having a fireplace in a single makes calculated rent less than base rent.

This is okay. Base rent is meant to be an index. As long as the user of the program knows, then it’s okay. If the program had help, I’m sure we’d put that in there!

All sizes of controls and form locations should be approximated. Please stick to MS-Sans Serif font for everything. The form itself should not be resizable.

Hints for Development

Remember you can set some initial properties using the properties window. You may also choose to explicitly set these options to their defaults by supplying some code in the Load event procedure for the form. This is a more professional way of doing it.

To create the numerous radio buttons on the form, it is necessary to draw the group box first before creation of the radio buttons that go inside it. Test these in the interface, making sure you’ve placed your buttons correctly and that they are properly “bound” to the appropriate group box. This doesn’t take any special command, just proper graphic placement.

Development in VB is very different from C or other procedural languages. You can test your creation at any time by pressing F5 and running it. Do a little at a time. You will end up with lots of event procedures, but that’s the nature of VB.

Try to come up with a coherent algorithm for determining the rent. Some of you may try to do the calculations all when the button is clicked. Others of you will change the values of certain “offset amount” variables as you change the options. It’s up to you (although the first way is probably easiest for most of you). The important thing? It better work and give the right answers!

This is a program that CRIES for code subroutines (other than the many event subroutines), defined constants, and good commenting. Make sure you do so!

You should also try to distinguish properly between text boxes, labels and actual variables. Use variables for your calculating, text boxes for input, and labels for display. Remember, you can make a label look like a textbox (except it doesn’t allow users to get the value); please do this when necessary. Name your objects other than the default (in other words, don’t use Label1, Combo1). Give meaningful names and use the naming conventions we discussed in class.

Don’t worry about a formal design for this program; you won’t be handing one in. HOWEVER, you should still do some design work. I’d use some form of pseudocode or Nassi-Schneiderman chart for each event procedure just to indicate what the program is to do when.

Skyforest Naming Conventions

Please use the following conventions for naming your Skyforest form. The file name is based on a fictional student named Jenny Chen, so you should use your own first initial and last name.

Internal form name: frmSkyforest (only the S is capitalized)

File name example: frmJChen_sky.vb

The designer file will be created automatically, and will be called (as an example): frmJChen_sky.Designer.vb

These naming conventions must be followed for this assignment, or your points will be affected.

What and How to Submit

Your final submission to me should be your form file (.vb file) AND your designer file (Designer.vb file). We will run the application and test it for accuracy and proper operation. You will receive up to 5 points for this assignment.

Please submit only the specified file(s) via the assignment submission area on the Blackboard web site for this course. Do not submit any of the other files generated. Do not email the files to me. If you need to resubmit one or more files due to an error in the original submitted file(s), then you must email me to request that I “reset” your submission. Try your best, however, to submit only one final version. If you do submit more, the last one submitted prior to the due date is the one that will count for the grade. Please check the announcements for the due dates and announcement of spec changes and clarifications.

PAY CLOSE ATTENTION TO THE FOLLOWING: DO NOT SUBMIT THE .vbproj FILE OR .sln file OR ANY OF THE OTHER FILES GENERATED. YOU MUST SUBMIT THE .vb FILE (representing the form) AND THE .Designer.vb file BY THE DUE DATE OR YOU WILL RECEIVE A SCORE OF ZERO FOR THIS ASSIGNMENT. We cannot execute a .vbproj file or .slnfile or any of the others because they don’t have code in them. And while we can run an .exe file, we can’t grade it because there is no code to grade.




Words to the Wise

This is your first “big” Visual Basic program, and yes it is quite “rich” and full of details. But you’ve been through some C and VB programming now and see what’s needed to map the real world into some code. You saw in class the VB syntax is fairly easy, and this program uses only the most basic of statements. The key is here to pay attention to the details. Get the numbers right; that’s of utmost importance. Secondly, get the user interface right. Test, test, test, test, test your program! For those things that are a bit sticky, if you need a nudge, send me an email and I’ll try to help you out.0