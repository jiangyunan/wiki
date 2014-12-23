###File类

####位置
java.io包

####功能
新建，删除，重全名文件和目录，不能访问文件本身

####方法
| 方法名 | 功能 | 
| ---- | ---- |
| String getName | 返回File名或最后一级子路径名 |
| String getPath | 返回此File全路径名 |
| File getAbsolutePath() | 返回绝对路径名|
| File getAbsoluteFile() | 返回绝对路径的File对象 |
| String getParent() | 父目录名 |
| boolean renameTo(File newName) | 重全名 |
| boolean exists() | 判断File是否存在 |
| long lastModified() | 最后修改时间 |
| long length() | 内容长度 |
| boolean createNewFile() | 当File不存在新建一个File文件 |
| boolean delete() | 删除File对应的文件或目录 |
| static File createTempFile(String 前缀, [String 后缀, File 指定目录]) | 在默认的临时文件中创建一个临时的空文件 |
|  void deleteOnExit() | 注册一个钩子，Java虚拟机退出删除File |
| boolean mkdir() | 创建File所在的对应目录 |
|String[] list() | 列出子文件名和路径名 |
|static File[] listRoots() | 列出系统所有的根 |

###字节流与字符流

####InputStream  Reader
输入流抽象基类，都有`read`方法