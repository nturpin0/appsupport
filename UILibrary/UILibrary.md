You can use UI Library to show more formatted information with nicer fonts without having to add a template to your Shortcut each time, or to show a Markdown/html table. Or to choose a Shortcut(with Search), choose a color, easily show a list of percentages, or a list with images in the menu. 

All of these are done with 2/3 actions added to your Shortcut.

Try the Demo once you've installed the library.





## ShowCard
Card has a blue title block, where you can put an icon, and a title. If you put an image in Image is displayed first with title, and any text below. Markdown wont work inside the card.

- Process: ShowCard
- Background: Background color
- Icon: (optional) Name of icon to be shown. Icons are from font-awesome, and require the font-awesome name eg book-open, home.
- Title: Title to be shown on card, and at the top of the quickview window.
Text: TExt to be shown on card.
Image: Base64 encoded image (optional)

## Show Result
- Process: Show Result
- Title: Title to be shown at top of the quickview window
- Background: Bacground color, you can use web color names, or hex values
- TextColor: Color of text, web color names.
- Text: Text to be shown, this can include Markdown.

## ShowTable
- Process: ShowTable
- Title: Title to be shown on the quickview window.
- Text: Text containing the html or Markdown to be displayed
- Type: HTML/Markdown

## Choose Shortcut
- Process: Choose Shortcut
- Title: Text to be shown above the choose box.

## ColorPicker
This was originally done, by @heyitzspencer
- Process: ColorPicker
- Choose colors, or enter a hex value.

## PercentageBars
- Process: PercentageBars
- Title: Title to be shown above the list
- Data: Data to be shown

Data should be in the following format 

Subtitle,number

eg 
Q1 Sales,67

## MenuList
MenuList
Send lines of text to show a list with images, or just use it for a left justified menu with no images.

- Process: MenuList
- List: list to be shown, 
- Title: Title to be shown at the top of the list displayed.

Lists should be sent in the following format, images are optional if you just want left justified menus.
- Title, subtitle, Base64EncodedImage

If not using subtitles, commas should be kept in image
- Title, , Base64EncodedImage



## Distributing Your Shortcuts
If using in a Shortcut you want to distribute to people, they will also need to have the library installed look at using 

DependKit by @heyitzspencer allows shortcuts to require certain dependencies to run
BundleKit by @medicalshortcut helps automatically create a bundle installer shortcut to install all dependencies at once
