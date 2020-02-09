# File System

All computers or smartphones have memory to store data. In this lesson we will briefly cover how that data is stored in a hard drive and how we can have access to it.

## Concepts

- Filenames: They are names that represent a storage location in a hard drive.
- Directories: They are a name that represent a group of files or other directories. 

## Think of a tree
Imagine filenames are flowers and directories are trees. Your hard drive is a place with some ground (physical space) where you can plant as many flowers and trees as they fit.
You can think of this ground as the main drive directory. In Windows this is usually represented as `C:\` but could be any other letter. In linux systems would be `/`.

So a hard drive could look like:

```
.
├── rose.jpg
├── begonia.png
├── magnolia.jpg
├── trip_to_spain
│   ├── madrid.jpg
│   ├── madrid.doc
│   └── madrid-1.jpg
├── trip_to_barcelona
│   ├── bcn.doc
│   └── bcn.xls
├── other
│   └── unordered_stuff.txt
├── Windows
│   ├── System
│   │   └── Something
│   └── Program Files
│       └── Some file
└── ...
```

### Want to see yours?
1. Open a terminal (Ctrl + Alt + T) in linux or search for Power Shell in windows.

**Windows** or **Linux**

- `tree`

**Mac**

- `find . -print | sed -e 's;[^/]*/;|____;g;s;____|; |;g'`

2. You should see a tree like the one we drew.

## Accessing files

### User interface
To open and save your files, you normally use a user interface, a file manager like windows explorer or nautilus in linux or finder in mac. You open any folder and you can navigate through it subfolders by clicking. Or even when you are prompted to save a file when you download it or you create it for the first time.

### The path
But what is going underneath? 
What you see in the user interface is just a beautiful representation of the path of files and directories. But, how does this path look like? Don't worry, you can find these paths everywhere. Lets place an example:

In the tree we previously drew this is how a path would look like for the madrid picture inside trip to madrid folder and a magnolia photo in the root of the hard drive:

#### Absolute path
In windows: `C:/trip_to_spain/madrid.jpg`, `C:/magnolia.jpg`
In linux and mac: `/trip_to_spain/madrid.jpg`, `/magnolia.jpg` 

We just draw the absolute path. This means, that is the path relative to the root of the hard drive, remember, `C:/` in Windows and `/` in linux.

#### Relative path
But we could also refer to a file with a relative path, for example, if wanted to know the path of magnolia photo in the root related to the madrid photo in the trip to spain directory:

In windows and in linux: `../magnolia.jpg` 

Weird? Its just a convention. When speaking about realtive routes you need to know the following:

`.` When you see a single dot, it means its the place where we are in the moment of writing it. At the same level of whatever its relative to.
`/` You saw this before to specify that a directory or a file is under/inside another.
`../` Single dot ment that you where in the same place than the related file. This one means you are referring to a previous/upper file or directory.

Examples:

Related to `/Windows/Program Files/Some`: 
- `../System/Something`
- `../../other/unordered_stuff.txt`
- `../../trip_to_barcelona`.


Related to `other/unordered_stuff.txt`: 
- `.../Windows/System/Something` 
- `../trip_to_barcelona`.

## Lets try it!

1. Open a terminal (Ctrl + Alt + T) in linux or search for Power Shell in windows.
2. Type `pwd` and press enter
3. You should see a result with the absolute path indicating where you are in the hard drive. By default, `C:/Users/YourUser` in windows and `/home/YourUser` or `~/YourUser` in linux. `~/` stands for "the default user directory"
4. Now, type `ls -l` and press enter
5. You should see a list of the files and directories relative to where you are in the hard drive. 


## Other Paths

Now you know what is a path and how it looks like, you will realise there are other places where you can find them. For example in websites, when you type in: `www.domain.com/contact`.  Its an absolute path where the domain would act as root (instead of `C:/`) and the **/contact** would be _like_ a file inside it.

## If you didn't understand everything

[Read this](http://resources.esri.com/help/9.3/ArcGISDesktop/com/Gp_ToolRef/sharing_tools_and_toolboxes/pathnames_explained_colon_absolute_relative_unc_and_url.htm)

## Related bibliography

- https://en.wikipedia.org/wiki/Path_(computing)
- https://en.wikipedia.org/wiki/File_system
- https://docs.microsoft.com/en-us/powershell/
- https://www.gnu.org/software/bash/
  