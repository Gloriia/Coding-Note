# Coding-Note

1.uploading folder in github : https://www.youtube.com/watch?v=wXGa0bDvFWA  

2.3%的代码占用了80%的时间，python profile可以排查 : https://docs.python.org/2/library/profile.html
(什么语言都有profile可查)

3.train = pd.read_csv('../train.tsv',encoding='utf-8')
报错：ParserError: Error tokenizing data. C error: Expected 2 fields in line 83, saw 3
改为：train= pd.read_csv("../input/train.tsv", sep="\t")
