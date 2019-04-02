# Tagger


TO COMPLETE LIST
Default File Location
Reminder View


Tagger is for managing your set of tags, searching them, or creating a new tagged item.
It works with Calendar, Contacts, Notes, and Reminders, or you can use functions from it in other Shortcuts so it can work with more apps.


## Select/Manage tags
Select tags to search, or to create a new item, quickly see how many matches there are for each tag and type, or manage your tags.
￼![](/img/one.png)

## Search results
Detailed previews where you can jump to an item you select (Reminders will only preview) 
Match counts and visual indicators.
Search looks for incomplete reminders/future calendar dates, all notes and all contacts.
￼￼![](/img/two.png)

## Create new item with selected tag(s)
You dont need to create tagged items from here, add them at any time to an item.
￼![](img/three.png)


## Use in your own Shortcuts
All you need to do is send a Dictionary with a key of function, and value of ShowTagList, and the tag selection/manage menu will show and return the tags selected. 

Tags are returned as a list, so may need some additional actions depending on which app your using.

Here’s two examples where you can select from your main tags.txt list to create a new tag in Bear, or Drafts using the ShowTagList function below. 

[https://www.icloud.com/shortcuts/fb77073a0f3240a3859461361e243273](Drafts Tagger example) 
[https://www.icloud.com/shortcuts/dd3b04d75ef447548a6f4e38df149665](Bear Tagger example)


Tags are held in icloud/Shortcuts/tags.txt


Functions

### ShowTagList
Shows a list of the current tags along with counts of the number of matching Notes, Contacts, items, and allows you to select one, or to use the ManageTags.

function : ShowTagList


### Search
Will return a list of Contacts, Notes, Reminders and Calendar items that are tagged with the submitted tag. Whilst it search on multiple tags it will return any items with both search terms in twice.

```
function : Search
tag : 
```

### New Item
New Contact, Note, Reminder or Calendar item with any tag/tags submitted.

```
function : NewItem
tag : 
```

### GetTagsFile
Will return the tags from the tag file, or ask you to create a new tag file if none exists.
```
function : GetTagsFile
```
