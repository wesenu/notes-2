[](...menustart)

- [python tips (most 2.7)](#149b164aabd9e2da3e4ff789cbfefe85)
    - [语法技巧](#cd82da5cf3ee760792e950b087be3d29)
        - [Print without new line](#28f6845e60c8649924fd266be2fd408b)
        - [eval 字符串表达式求值](#5a80441c284c199eaf6f839c5210a986)
        - [获取变量x的内存地址](#f372cdc8f82db5bb3a311edc6743e412)
        - [for i, v  枚举](#5bd260e9c2d18f7f2ff4c30f274ebc6b)
        - [min return both value and index](#898381b273cf9617a8b33660e4e27953)
        - [数组排序](#d4c8995bb39e2f93cb9604c56fa777d5)
        - [字典排序 sorted](#ab7c2e3bc42c80125290e5763dcad146)
        - [迭代和组合](#7b6bcc5e50cc1ddd83a25620f5739920)
        - [bisect模块保持列表排序](#04539cb02f80127546f36cb81567946d)
        - [url unescape](#18bf7f45d4c0960b7a240195d229cdbc)
        - [html escape](#c438002415894d6f16a66c0f4af9a454)
        - [序列 ()](#1c65ec66e824c6ab4c57603cf633a25d)
        - [自省的核心 getattr 函数](#95cc82c5a8eea453d65f25f13121bd7c)
        - [callable](#765d2ec94553b7cf4c971e7dfcf0e851)
        - [dict get](#f3fb87677ab41e55ff2069660fddcebf)
        - [dict setdefault](#f911a4fc9f3eb152b05e1a9f4b9269a2)
        - [dict insection](#2292cf7bac8199cfa91cb22160b26f76)
        - [dict key/value 反转](#734d33eb4b09a4486fff62a4f1498c3c)
        - [convert a list to dict](#51e210523bb6691db8601ee6c34f89d9)
        - [python2 unicode 判断](#2eef1e426b799acf96d762b3dc95a051)
        - [方法内全部局部变量](#76a7e51a79a55462350aaed109577894)
        - [输出一个对象各个成员的名称和值](#dd6b35cfcf7bc2919f28aaba9e65fa92)
        - [python 下划线变量](#379e1d911a58f6e847ad68e52703c7eb)
        - [re.sub group: number after \number](#8160fc3170b680fdd05d32a93937bcb9)
        - [call super class constructor](#7bb8886dc369a3137b7dd907c9ff7993)
        - [numpy argmax tie breaking](#4330cb83a720d5c17727f9762bff14cd)
    - [数字进制转换](#4155a2d7d71ebf1611555bda413d2961)
        - [10进制数字 => 2,8,16进制字符串](#4b65978fe4cba7b22aecf6375e8737db)
        - [2,8,16进制字符串 ==> 10进制数字](#819934946947aa7e3778247b469c1e4c)
        - [格式化数字为16进制字符串](#44ecb2e9ff829c50b0b0f9f4e9f7b918)
    - [字符处理](#fa931b43907b0ba8b8616487e1a14097)
        - [ascii列表 -> 字符串](#47785be60ccbe583a8c3f8a1c3b80d00)
        - [字符串编码相关](#5eee76378b49e64c0a5f5d768463fca6)
            - [python2 unicode/str convert](#f107f4274b339136846a24463f2ff9c4)
            - [char / ascii 互转](#a8f764cb43760ccd122114ec8679789b)
            - [python2 unichr / unicode string 互转](#3818367ee9105c0ed47b92186ebd3f00)
            - [python2 unicode -> special encoded string](#e7358efa47ced51b6ce16b4f866186af)
            - [python2 special encoded string -> unicode](#676299737b912fa0f3b8125df27a4b42)
            - [convert '\\n' to '\n'](#56932c830dacb8440022cdb350ae3bca)
    - [中文处理](#c4e5abc4816842dea936c9f1f20b431e)
        - [改变脚本本地编码](#7ab8dd9eb1e1a86afb68efff05a2e355)
        - [python 2.7 写 带中文字符的文件](#0bb0682eeb96c4d4d73977c7efd15c17)
        - [Json dump, indent + sort keys](#355832ef6c55cf7c4768f66e8996697d)
        - [python2 获取中文字符长度](#a2922e028e26838bcbaa6cb5d9cb57dd)
    - [encrypt](#53c82eba31f6d416f331de9162ebe997)
        - [base64](#95a1446a7120e4af5c0c8878abb7e6d2)
        - [md5](#1bc29b36f623ba82aaf6724fd3b16718)
        - [CRC32 IEEE](#d86a76b0e9825d4420259cf836f9230a)
        - [Base58](#0f3fed443cef1a400f3ac44edebf896b)
    - [Misc](#74248c725e00bf9fe04df4e35b249a19)
        - [try - except 打印错误](#636a8076c1d8da426394e0c3e15c3ec2)
        - [python 并行任务技巧](#eadbf8dd738ffd6eb430b8630c92d74c)
        - [profile](#7d97481b1fe66f4b51db90da7e794d9f)
        - [强制浮点数运算](#74343fa59d92ff47cbb14750228abd8f)
        - [float -> IEEE 754](#05226bcb71c2e5f63900d9f304161387)
        - [int -> Binary](#43cf8bc0b68f7fc42c32645065656365)
        - [读取文件特定行](#210dd2176d44f2bd7f0c112101e62490)
        - [文件修改／创建时间](#4b373365b500e18ab7c0b8f5a83dc802)
        - [python 写 只读文件](#3fbb096fc383c2a61ad0a6685b17c0de)
        - [uninstall files via `python setup.py install`](#5a3fb21375ecbb14ce59ad950a4b5f49)
        - [enter interact mode after executing a python file](#e3c3e4edeeaec5c36e52fe88b8fd33fe)
        - [add python module search path](#c005e12b106174340f49500f7c1ab309)
        - [open file with both reading and writing](#b8976c77d38eafc77157b35d8969c262)
        - [basis of Datetime and Time](#fdbe9d1605732955d440487ba60d2368)
        - [seconds to readable date](#ec96030c0279fc4c33c1d008de5222c0)
        - [convert between seconds since the epoch  and  struct_time](#fb28c08f40bf7d1c5542c312b46232c8)
        - [Determining application path in a Python EXE generated by pyInstaller](#3fea1af701d185d74668117c9555eb60)
        - [subprocess](#c246f93a794588f0eff7e71b3e981790)
        - [python 解析 curl 命令获取的 json 字符串](#c88f2db1064b41d03c5779d4ef9aef26)
        - [memoize decorator](#66fc7c7caa9e9bf96224fa5b044a0251)

[](...menuend)


<h2 id="149b164aabd9e2da3e4ff789cbfefe85"></h2>

# python tips (most 2.7)

---

<h2 id="cd82da5cf3ee760792e950b087be3d29"></h2>

## 语法技巧

<h2 id="28f6845e60c8649924fd266be2fd408b"></h2>

### Print without new line 

```python
for i in range(5):
    # return only, no new line
    print( i, end="\r" )
```

```
4
```

```python
for i in range(5):
    # no return, no new line
    print( i, end="" )
```

```
01234
```


<h2 id="5a80441c284c199eaf6f839c5210a986"></h2>

### eval 字符串表达式求值 

eval() 默认使用当前环境的名字空间，也可以带入自定义字典

```
ns=dict(x=10,y=20)
eval("x+y" , ns )
```

eval只能用来处理表达式, 对于 代码段, 可以使用 `exec()`


<h2 id="f372cdc8f82db5bb3a311edc6743e412"></h2>

### 获取变量x的内存地址

```
id(x) 
```

<h2 id="5bd260e9c2d18f7f2ff4c30f274ebc6b"></h2>

### for i, v  枚举

```
for i, item in enumerate(  iterable ):
```

<h2 id="898381b273cf9617a8b33660e4e27953"></h2>

### min return both value and index 

```python
mport operator
>>> scores = [30, 10,20 ]
>>> min(enumerate(scores ), key=operator.itemgetter(1))
(1, 10)
```


<h2 id="d4c8995bb39e2f93cb9604c56fa777d5"></h2>

### 数组排序

```python
# .sort(), in-place sort, return None
autodances.sort( key = lambda x  :  x["time"] , reverse = False )
```

use `cmp` method . (PS. **deprecated in python3** )

```python
# python2 only
l.sort(cmp=lambda x,y:cmp( x.lower(), y.lower()  ))
```

<h2 id="ab7c2e3bc42c80125290e5763dcad146"></h2>

### 字典排序 sorted

```
>>> d={"b":2, "a":3, "c":1}
>>> sorted(d)     #对 key 进行排序，输出一个key list
['a', 'b', 'c']      
>>> sorted(d.iteritems())     #对key 进行排序，返回 元组 list
[('a', 3), ('b', 2), ('c', 1)]
>>> sorted(d.iteritems() , key=lambda x:x[1])    # 对 值 进行排序， 返回 元组 list
[('c', 1), ('b', 2), ('a', 3)]
>>> sorted(d.iteritems() , key=lambda x:x[1] , reverse = True )
[('a', 3), ('b', 2), ('c', 1)]
```


<h2 id="7b6bcc5e50cc1ddd83a25620f5739920"></h2>

### 迭代和组合

了解itertools模块：  该模块对迭代和组合是非常有效的

```
>>> import itertools 
>>> iter = itertools.permutations([1,2,3]) 
>>> list(iter) 
[(1, 2, 3), (1, 3, 2), (2, 1, 3), (2, 3, 1), (3, 1, 2), (3, 2, 1)]
```

<h2 id="04539cb02f80127546f36cb81567946d"></h2>

### bisect模块保持列表排序

这是一个免费的二分查找实现和快速插入有序序列的工具。你已將一个元素插入列表中, 而你不需要再次调用 sort() 来保持容器的排序, 因为这在长序列中这会非常昂贵. 

```
>>> import bisect 
>>> bisect.insort(list, element) 
```


<h2 id="18bf7f45d4c0960b7a240195d229cdbc"></h2>

### url unescape


```python
import HTMLParser
html_parser = HTMLParser.HTMLParser()
txt = html_parser.unescape(html)
```

```python
import urllib
urllib.unquote(a)
```

```python3
# for python3
urllib.parse.unquote(url)
```


<h2 id="c438002415894d6f16a66c0f4af9a454"></h2>

### html escape 

```python
>>> print cgi.escape.__doc__
Replace special characters "&", "<" and ">" to HTML-safe sequences.
    If the optional flag quote is true, the quotation mark character (")
    is also translated.

>>> import cgi
>>> cgi.escape( '>' )
'&gt;'
>>> cgi.escape( '"' , True )
'&quot;'
```





<h2 id="1c65ec66e824c6ab4c57603cf633a25d"></h2>

### 序列 ()  

速度比列表快，  可以作为字典关键字

<h2 id="95cc82c5a8eea453d65f25f13121bd7c"></h2>

### 自省的核心 getattr 函数

```
getattr(obj, name [ ,  default_method_return_if_not_exist ] )

example:

for i in  dir( obj ):
    method = getattr( obj, i   )
    print i , method
```

<h2 id="765d2ec94553b7cf4c971e7dfcf0e851"></h2>

### callable

```
methodList = [method for method in dir(object) if callable(getattr(object, method))]
```

<h2 id="f3fb87677ab41e55ff2069660fddcebf"></h2>

### dict get

从字典中获取一个值 

```
if d.has_key('key'):
    print d['key']
else:
    print 'not found'
```

可以简化为:

```
print d.get('key', 'not found')
```    

<h2 id="f911a4fc9f3eb152b05e1a9f4b9269a2"></h2>

### dict setdefault

dict 插入key-value时，如果key不存在，先初始化为默认值(一般用于value是list, dict 类型)

```
def addword2dict(word, pagenumber): 
    dict.setdefault(word, []).append(pagenumber)
```

或者直接使用  defaultdict

```
from collections import defaultdict
d = defaultdict( dict )  # default value is empty dict
d = defaultdict( lambda: 2 )  # default value is 2

```

<h2 id="2292cf7bac8199cfa91cb22160b26f76"></h2>

### dict insection

找出两个字典的交集 

```
print "Intersects:", [k for k in some_dict if k in another_dict]
```

速度上取胜:

```
print "Intersects:", filter(another_dict.has_key, some_dict.keys())
```

<h2 id="734d33eb4b09a4486fff62a4f1498c3c"></h2>

### dict key/value 反转

```python
>>> m = {"a":1,"b":2,"c":3}
>>> dict( zip( m.values(), m.keys() ) )
{1: 'a', 2: 'b', 3: 'c'}
```

or

```python
>>> {v:k for k,v in m.iteritems() }
{1: 'a', 2: 'b', 3: 'c'}
```

<h2 id="51e210523bb6691db8601ee6c34f89d9"></h2>

### convert a list to dict 

```python
>>> a = [3,1,2,4]
>>> dict(  zip(  *[iter( a )] *2  )  )
{3: 1, 2: 4}
```

or more simple

```python
i = iter(a)
dict(zip(i, i))   # you must use a single iterator 
```

<h2 id="2eef1e426b799acf96d762b3dc95a051"></h2>

### python2 unicode 判断

```python
# python2
isinstance(u'a', unicode)
```

<h2 id="76a7e51a79a55462350aaed109577894"></h2>

### 方法内全部局部变量

Python has a locals() function which gives you back a dictionary of local variables within the function



<h2 id="dd6b35cfcf7bc2919f28aaba9e65fa92"></h2>

### 输出一个对象各个成员的名称和值

```
>>> g = lambda m: '\n'.join([ '%s=%s'%(k, repr(v)) for k, v in m.__dict__.iteritems() ])
>>> g(obj)
```


<h2 id="379e1d911a58f6e847ad68e52703c7eb"></h2>

### python 下划线变量

核心风格：避免用下划线作为变量名的开始。

- `_xxx`      
    - 不能用'from module import \*'导入 
    - **保护变量**，意思是只有 类对象和子类对象自己 能访问到这些变量
- `__xxx`    
    - 类中的私有变量名
    - **私有成员**，意思是只有类对象自己能访问，连子类对象也不能访问到这个数据
- `__xxx__`
    - 系统定义名字 
    - python里特殊方法专用的标识

<h2 id="8160fc3170b680fdd05d32a93937bcb9"></h2>

### re.sub group: number after \number

```
re.sub(r'(foo)', r'\1123', 'foobar') 
=>
re.sub(r'(foo)', r'\g<1>123', 'foobar')
```


<h2 id="7bb8886dc369a3137b7dd907c9ff7993"></h2>

###  call super class constructor

```python
def __init__(self) :
    super( self.__class__ , self).__init__()
```


<h2 id="4330cb83a720d5c17727f9762bff14cd"></h2>

### numpy argmax tie breaking 

```python
b = np.array( [0,1,1] )
np.random.choice(np.where(b == b.max())[0])
```

or 

```python
np.random.choice(np.flatnonzero(b == b.max()))
```

- b == b.max() will return an array of boolean, with values of true where items are max and values of false for other items
- flatnonzero() will do to things: ignore the false values (nonzero part) then return indices of true values. In other words, you get an array with indices of items matching the max value
- Finally, you pick random index of these




----------


---

<h2 id="4155a2d7d71ebf1611555bda413d2961"></h2>

## 数字进制转换

<h2 id="4b65978fe4cba7b22aecf6375e8737db"></h2>

### 10进制数字 => 2,8,16进制字符串

```python
>>> bin(123) # 2
'0b1111011'
>>> oct(18) # 8
'0o22'
>>> hex(10) # 16
'0xa'
```

<h2 id="819934946947aa7e3778247b469c1e4c"></h2>

### 2,8,16进制字符串 ==> 10进制数字 

```python
>>> int('022',8) 
18
```

<h2 id="44ecb2e9ff829c50b0b0f9f4e9f7b918"></h2>

### 格式化数字为16进制字符串

```
>>> "%x" % 108
'6c'
>>>
>>> "%X" % 108
'6C'
>>>
>>> "%#X" % 108
'0X6C'
>>>
>>> "%#x" % 108
'0x6c'
```

---

<h2 id="fa931b43907b0ba8b8616487e1a14097"></h2>

## 字符处理

<h2 id="47785be60ccbe583a8c3f8a1c3b80d00"></h2>

### ascii列表 -> 字符串

good 1

```
import string
def f6(list):
    return string.joinfields(map(chr, list), "")
```

the best 1

```
import array
def f7(list):
    return array.array('B', list).tostring()
```

<h2 id="5eee76378b49e64c0a5f5d768463fca6"></h2>

### 字符串编码相关


<h2 id="f107f4274b339136846a24463f2ff9c4"></h2>

#### python2 unicode/str convert

- string -> decode -> unicode 
- unicode -> encode -> string 

<h2 id="a8f764cb43760ccd122114ec8679789b"></h2>

#### char / ascii 互转

```
>>> print ord('a')
97
>>> print chr(97)
a
```

`'2' == '\x32' == '\062'`

<h2 id="3818367ee9105c0ed47b92186ebd3f00"></h2>

#### python2 unichr / unicode string 互转

```
>>> print ord(u"我")
25105
>>> print unichr( 25105 )
我
```

<h2 id="e7358efa47ced51b6ce16b4f866186af"></h2>

#### python2 unicode -> special encoded string

```
unicodestring = u"Hello world"
utf8string = unicodestring.encode("utf-8")
asciistring = unicodestring.encode("ascii")
isostring = unicodestring.encode("ISO-8859-1")
utf16string = unicodestring.encode("utf-16")
```

<h2 id="676299737b912fa0f3b8125df27a4b42"></h2>

#### python2 special encoded string -> unicode

```
plainstring1 = unicode(utf8string, "utf-8")
plainstring2 = unicode(asciistring, "ascii")
plainstring3 = unicode(isostring, "ISO-8859-1")
plainstring4 = unicode(utf16string, "utf-16")
```

unicode 可以使用 u"\uxxxx" 表示，但是当我们从某处获取 "\uxxxx"， 并不能直接还原成 unicode，需要通过  "\uxxxx".decode("unicode-escape") 来转成 unicode， 注意， xxxx 必须保证有4个，不足以0补全

反之 ，通过  uni.encode("unicode-escape")  来 获得 "\uxxxx"  形式的字符串


<h2 id="56932c830dacb8440022cdb350ae3bca"></h2>

#### convert '\\n' to '\n'

```python
>>> "\\n"
'\\n'
>>> "\\n".decode('string_escape')
'\n'
```


---

<h2 id="c4e5abc4816842dea936c9f1f20b431e"></h2>

## 中文处理

<h2 id="7ab8dd9eb1e1a86afb68efff05a2e355"></h2>

### 改变脚本本地编码

- 有时候，print 打印某些unicode字符的时候，会报 UnicodeError

```
reload(sys)
sys.setdefaultencoding('utf8') 
```

<h2 id="0bb0682eeb96c4d4d73977c7efd15c17"></h2>

### python 2.7 写 带中文字符的文件

```
fp = codecs.open( target_sheet_name + '.txt'  , "w", "utf-8")
fp.write(jsonObj )
fp.close()
```


<h2 id="355832ef6c55cf7c4768f66e8996697d"></h2>

### Json dump, indent + sort keys

```python
json.dump( obj, fp, ensure_ascii=False , separators=(',',':') , indent=4, sort_keys=True  )  
```

<h2 id="a2922e028e26838bcbaa6cb5d9cb57dd"></h2>

### python2 获取中文字符长度

- 需要转成unicode字符

```
unicode_string = bytes.decode("utf-8")
print len(unicode_string)
```

---

<h2 id="53c82eba31f6d416f331de9162ebe997"></h2>

## encrypt

<h2 id="95a1446a7120e4af5c0c8878abb7e6d2"></h2>

### base64

```
import base64
# base 64 decode
data = base64.b64decode( data ) 
# base64 encode
result_data = base64.b64encode( result_data)
```

<h2 id="1bc29b36f623ba82aaf6724fd3b16718"></h2>

### md5

```
>>> import md5
>>> m = md5.new()
>>> m.update("Nobody inspects")
>>> m.update(" the spammish repetition")
>>> m.digest()
```


<h2 id="d86a76b0e9825d4420259cf836f9230a"></h2>

### CRC32 IEEE

```python
# python
import binascii
binascii.crc32(b"hello world")
```

```go
# go
import "hash/crc32"

crc32.ChecksumIEEE( []byte("hello world") ) )
```

<h2 id="0f3fed443cef1a400f3ac44edebf896b"></h2>

### Base58

```python
import base58
base58.b58encode( raw_str )
```

```go
import "github.com/btcsuite/btcutil/base58"
decoded := base58.Decode(b58_str)
```


---

<h2 id="74248c725e00bf9fe04df4e35b249a19"></h2>

## Misc

<h2 id="636a8076c1d8da426394e0c3e15c3ec2"></h2>

### try - except 打印错误

```python
import traceback
traceback.print_exc()
```

或者

```python
s=sys.exc_info()
print "Error '%s' happened on line %d" % (s[1],s[2].tb_lineno)
```


<h2 id="eadbf8dd738ffd6eb430b8630c92d74c"></h2>

### python 并行任务技巧

- 使用带有并发功能的map
- Dummy是一个多进程包的完整拷贝
- 唯一不同的是，多进程包使用进程，而dummy使用线程
- 简言之，IO 密集型任务选择multiprocessing.dummy(多线程) ， CPU 密集型任务选择multiprocessing(多进程)

```python
from multiprocessing import Pool
from multiprocessing.dummy import Pool as ThreadPool

pool = ThreadPool( poolsize )
results = pool.map( func ,  param_set_list  )
pool.close()
pool.join()
```

<h2 id="7d97481b1fe66f4b51db90da7e794d9f"></h2>

### profile

```
python -m cProfile  xxx.py
```

or

```
import profile
profile.run ( 'func_name')
```

<h2 id="74343fa59d92ff47cbb14750228abd8f"></h2>

### 强制浮点数运算

```python
>>> from __future__ import division
>>> 1/2
0.5
```


<h2 id="05226bcb71c2e5f63900d9f304161387"></h2>

### float -> IEEE 754


[online convert](https://www.binaryconvert.com/result_double.html?decimal=049)


```python
# use numpy
>>> b = bin( np.float32( 0.15625 ).view(np.int32) )
>>> b
'0b111110001000000000000000000000'
>>> expo, mantissa =  b[ -23-8:-23 ] , b[ -23: ]
>>> print(expo, mantissa)
('b1111100', '01000000000000000000000')
```


<h2 id="43cf8bc0b68f7fc42c32645065656365"></h2>

### int -> Binary


```python
>>> np.binary_repr( 200, width=8)
'11001000'
>>> np.binary_repr( -1, width=8)
'11111111'
```




<h2 id="210dd2176d44f2bd7f0c112101e62490"></h2>

### 读取文件特定行

```
import linecache
#thefiepath             文件路径
#desired_line_number    整数，文件的特定行 
theline = linecache.getline(thefilepath, desired_line_number)
```        

<h2 id="4b373365b500e18ab7c0b8f5a83dc802"></h2>

### 文件修改／创建时间

```
import   os,time 
time.ctime(os.stat( "d:/learn/flash.txt ").st_mtime)   #文件的修改时间 
time.ctime(os.stat( "d:/learn/flash.txt ").st_ctime)   #文件的创建时间
```

<h2 id="3fbb096fc383c2a61ad0a6685b17c0de"></h2>

### python 写 只读文件

读之前：

```
os.chmod(_path,  stat.S_IREAD)
```

写之前:

```
os.chmod(_path, stat.S_IWRITE | stat.S_IREAD)
```


<h2 id="5a3fb21375ecbb14ce59ad950a4b5f49"></h2>

### uninstall files via `python setup.py install`

```
python ./setup.py install --record install.txt

cat install.txt | xargs [sudo] rm -rf
```

<h2 id="e3c3e4edeeaec5c36e52fe88b8fd33fe"></h2>

### enter interact mode after executing a python file

```python
import code 

...
code.interact(local=locals())
```

<h2 id="c005e12b106174340f49500f7c1ab309"></h2>

### add python module search path

```python
src_path = os.path.dirname( os.path.abspath(  __file__ ) )
# add parent folder as search path
sys.path.append( os.path.normpath( os.path.join( src_path , ".." )) )
```


<h2 id="b8976c77d38eafc77157b35d8969c262"></h2>

### open file with both reading and writing 

```python
with open(filename, "r+") as f:
    data = f.read()
    f.seek(0)
    f.write(output)
    f.truncate()
```

<h2 id="fdbe9d1605732955d440487ba60d2368"></h2>

### basis of Datetime and Time

```python
import datetime as dt
import time as tm

# time returns the current time in seconds since the Epoch. (January 1st, 1970)
tm.time()
# 1511154150.7125366

# Convert the timestamp to datetime.
dtnow = dt.datetime.fromtimestamp(tm.time())
dtnow
# datetime.datetime(2017, 11, 20, 5, 3, 1, 695393)

# Handy datetime attributes:
dtnow.year, dtnow.month, dtnow.day, dtnow.hour, dtnow.minute, dtnow.second
# (2017, 11, 20, 5, 3, 1)

# timedelta is a duration expressing the difference between two dates.
delta = dt.timedelta(days = 100) # create a timedelta of 100 days
delta
# datetime.timedelta(100)

# date.today returns the current local date.
today = dt.date.today()
today - delta # the date 100 days ago
# datetime.date(2017, 8, 12)
today > today-delta # compare dates
# True
```

<h2 id="ec96030c0279fc4c33c1d008de5222c0"></h2>

### seconds to readable date 

```python
# here , `t` is  millis
>>> datetime.datetime.utcfromtimestamp( t/1000 ).strftime('%Y-%m-%dT%H:%M:%SZ')
'2019-03-01T09:33:08Z'
>>> datetime.datetime.fromtimestamp( t/1000 ).strftime('%Y-%m-%dT%H:%M:%SZ')
'2019-03-01T17:33:08Z'   # local time
>>> datetime.datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S.%f')[:-3]+"Z" 
'2019-09-19 07:56:37.326Z'
```

<h2 id="fb28c08f40bf7d1c5542c312b46232c8"></h2>

### convert between seconds since the epoch  and  struct_time

Use | From  | To
--- | --- | --- 
gmtime() | seconds since the epoch | struct_time in UTC
calendar.timegm() | struct_time in UTC  |  seconds since the epoch

Example:

```python
>>> calendar.timegm(  ( 2020,1,1,0,0,0 )  )
1577836800
>>> time.gmtime( 1577836800  )
time.struct_time(tm_year=2020, tm_mon=1, tm_mday=1, tm_hour=0, tm_min=0, tm_sec=0, tm_wday=2, tm_yday=1, tm_isdst=0)
```

<h2 id="3fea1af701d185d74668117c9555eb60"></h2>

### Determining application path in a Python EXE generated by pyInstaller

```python
# determine if application is a script file or frozen exe
if getattr(sys, 'frozen', False):
    application_path = os.path.dirname(sys.executable)
elif __file__:
    application_path = os.path.dirname(__file__)

config_path = os.path.join(application_path, config_name)
```

<h2 id="c246f93a794588f0eff7e71b3e981790"></h2>

### subprocess

- 使用subprocess模块
    - 这个模块比较复杂，可以对子进程做更多控制
    - Popen is nonblocking. call and check_call are blocking
    - `Popen(cmd , shell=True, cwd=  arg) .stdout.readlines()`
        - stdout=subprocess.PIPE , 会等待执行完毕再返回， 同时 原来脚本的 print ，都会从 stdout read 出来
    - 有些命令 ， 并不是从标准 stdout 输出结果，可以:
        - `res = subprocess.Popen( cmd , stdout=subprocess.PIPE  , stdin=subprocess.PIPE,  stderr=subprocess.STDOUT ,  shell=True ).stdout.read()`
    - TODO :  subprocess  Popen 指定 shell 执行路径
        - `print Popen(cmd , stdout=subprocess.PIPE  ,  shell=True, cwd=  arg)`  ?
    - 注： 如果没有 pipe 通讯的需求，推荐的用法如下
        ```python
        subprocess.call( cmd.split() +  sys.argv[1:]  , stderr=subprocess.STDOUT ,shell=True )
        ```
    - `shell=True` 是在 shell中执行，以便获取环境变量之类的设置
    - 如果需要获取 exit code
        ```python
        child = subprocess.Popen( cmd , stdout=subprocess.PIPE , stdin=subprocess.PIPE, stderr=subprocess.STDOUT , shell=True )
        streamdata = child.communicate()[0]
        rc = child.returncode
        ```

- Python3 subprocess.run
    ```python
    subprocess.run( [...] )
    ```
    - parent process will be blocked to wait child process to finish.
    - `catputre_output=True` to acquire the output
    ```python
    >>> import subprocess
    >>> result = subprocess.run( ["rm", "does not exist"], capture_output=True, shell=True )
    >>> result
    CompletedProcess(args=['rm', 'does not exist'], returncode=1, stdout=b'', stderr=b'rm: does not exist: No such file or directory\n')
    >>> print ( result.stdout )
    b''
    >>> print ( result.stderr.decode() ) # to utf8 by default
    rm: does not exist: No such file or directory
    ```

<h2 id="c88f2db1064b41d03c5779d4ef9aef26"></h2>

### python 解析 curl 命令获取的 json 字符串 

```bash
result=`curl --silent  ... | python -c "import json,sys;obj=json.load(sys.stdin);print obj['anykey'];"`
echo result: $result

```

<h2 id="66fc7c7caa9e9bf96224fa5b044a0251"></h2>

### memoize decorator

1. [implementation in Python Decorator Library](https://wiki.python.org/moin/PythonDecoratorLibrary#Memoize)
2. From python 3.2, `functools.lru_cache`
    - By default, it only caches the 128 most recently used calls, but you can set the `maxsize` to None to indicate that the cache should never expire:
    ```python
    import functools

    @functools.lru_cache(maxsize=None)
    def fib(num):
        if num < 2:
            return num
        else:
            return fib(num-1) + fib(num-2)
    ```



