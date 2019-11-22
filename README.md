# Coding-Note

1.uploading folder in github : https://www.youtube.com/watch?v=wXGa0bDvFWA  

2.3%的代码占用了80%的时间，python profile可以排查 : https://docs.python.org/2/library/profile.html
(什么语言都有profile可查)

3.train = pd.read_csv('../train.tsv',encoding='utf-8')
报错：ParserError: Error tokenizing data. C error: Expected 2 fields in line 83, saw 3
改为：train= pd.read_csv("../input/train.tsv", sep="\t")

4.在git clone的时候如果遇到报错：
remote: Enumerating objects: 128, done.
error: RPC failed; curl 18 transfer closed with outstanding read data remaining
fatal: The remote end hung up unexpectedly
fatal: early EOF
fatal: index-pack failed
那么：把http://改成git://,如下
git clone git://github.com/buppt/ChineseNER.git

5.如果有一个包怎么都无法跟环境兼容(版本不匹配之类的),那么重新写一个函数替代掉这个加载这个包要使用的函数就好了。
