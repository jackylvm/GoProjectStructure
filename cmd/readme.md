## cmd目录
* 项目主要的应用程序。
* 对于每个应用程序来说这个目录的名字应该和项目可执行文件的名字匹配（例如，/cmd/myapp）。
* 不要在这个目录中放太多的代码。如果目录中的代码可以被其他项目导入并使用，那么应该把他们放在/pkg目录。如果目录中的代码不可重用，或者不希望被他人使用，应该将代码放在/internal目录。显示的表明意图比较好！
* 通常来说，项目都应该拥有一个小的main函数，并在main函数中导入或者调用/internal和/pkg目录中的代码。