mdview
======
A live github flavored markdown viewer.

##### _NOTE:_ Following links in the preview doesn't always work.

### Compiling
Clone the repository:
```
git clone https://github.com/calvinhenderson/mdview
```

Change directory into the local copy:
```
cd mdview
```

Compile the project:
```
go build -ldflags -H=windowsgui -o mdview.exe src\main.go
```

### Usage
The program takes the path to the markdown file as the only argument.
```
mdview <markdown file>
```
A window will open showing the live preview. It updates automatically
whenever the file is written to.

### Dependencies
* <https://github.com/zserge/webview>       for webview window
* <https://github.com/russross/blackfriday> for markdown processing
* <https://github.com/rjeczalik/notify>	    for file system events