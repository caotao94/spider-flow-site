# file

## write

|    参数名     |               描述                | 可否为空 |
| :-----------: | :-------------------------------: | :------: |
|     path      |            写出的路径             |    否    |
| content/bytes/stream/List\<String> |       内容,字符串或字节数组或二进制输入流或url list       |    否    |
|    append     | 布尔类型,是否追加输出,默认为false |    是    |

::: tip 

无返回值

:::


- 写出文件,内容为`hello world!`

  ```javascript
  ${file.write('/data/test.txt','hello world!')}
  ```
## write

|    参数名     |               描述                | 可否为空 |
| :-----------: | :-------------------------------: | :------: |
|     path      |            写出的路径             |    否    |
|     urls      |       要下载的url集合      |    否    |

::: tip 

无返回值

:::


- 写出文件,批量下载文件

  ```javascript
  ${file.write('/data/',urls)}
  ```

## bytes

| 参数名 |       描述       | 可否为空 |
| :----: | :--------------: | :------: |
|  path  | 要读取的文件路径 |    否    |

::: tip 

返回值类型：byte[]

:::


- 读取`/data/test.txt`文件

  ```javascript
  ${string.bytes('/data/test.txt')}
  ```

## string

| 参数名  |         描述         | 可否为空 |
| :-----: | :------------------: | :------: |
|  path   |   要读取的文件路径   |    否    |
| charset | 编码格式,默认为UTF-8 |    是    |

::: tip 

返回值类型：String

:::


- 读取`/data/test.txt`文件

  ```javascript
  ${string.string('/data/test.txt')}
  ```
  