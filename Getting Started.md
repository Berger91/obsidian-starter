# Getting Started

## Keyboard Shortcuts

`CMD + O` - Find and Open file  
`CMD + P` - Command Palette  
`CMD + Shift + ;` - Open weekly note  
`CMD + Shift + [` - Previous weekly note  
`CMD + Shift + ]` - Next weekly note  
`CMD + Enter` - Switch task status (starts from uncompleted task)

## Change Theme

1. Open obsidian options using ⚙️ or `CMD + ,`
2. Go to Apperance -> Themes -> Manage  
   ![[Pasted image 20230228084016.png]]
3. Find and use theme of your choice  
   ![[Pasted image 20230228084048.png]]

## Playing with Tasks

1. Use `CMD + Enter` to create and complete tasks
	1. [ ] Created
	2. [x] Completed ✅ 2023-02-28
2. Recommended: Use tags for better task management
	1. [ ] #example-tag Task that we can find easily
3. Use dataview queries to aggregate task from multiple directories and files  
https://blacksmithgu.github.io/obsidian-dataview/  

Example:

```dataview
TASK FROM "Getting Started"
WHERE !completed AND contains(text, "#example-tag")
SORT file.ctime DESC
GROUP BY file.ctime
SORT rows.file.ctime DESC
```

## Daily Flow

Personally I use Weekly notes to aggregate/collect task & topics during the week.

I use tags directly in tasks, notes, meeting notes and everywhere where text reffers to any specific topic. That helps to find and link thoughts between distributed files.  
Other option is to group them is to use backlinks to specific file, like [[README]]

For more targeted topics I use dedicated notes grouped under directories (Projects, Technical notes etc.)

## Read It Later

Every article that I would like to read later, I save using ReadItLater plugin.

To use it copy link to the system clipboard and invoke plugin command  
![[Pasted image 20230228092817.png]]

## How to Paste Images inside Notes

Use `CMD + V` directly in notes. Current configuration store all attachments in `attachment` folder in the same place where the specific note is. 