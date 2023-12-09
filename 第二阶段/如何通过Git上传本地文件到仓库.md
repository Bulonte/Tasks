# 如何通过Git上传本地文件到仓库

## 1.创建密钥并与Github链接

在Git bash 中输入

```
ssh-keygen -t rsa
```

从而生成一个密钥，然后在本地文件中找到一个.pub后缀的文件用记事本打开，将密钥添加到Github上

## 2.创建一个本地仓库

依次输入以下指令

```
mkdiv <仓库名>

cd  <仓库名>

pwd

git init
```

## 3.创建一个文件放入本地仓库中

创建完后用以下指令将该文件送入暂存区

```
git add 文件名.后缀

git commit -m "说明"
```

## 4.关联仓库

依次输入以下指令关联仓库

```
git remote add origin git@github.com:<远程仓库地址>.git
```

## 5.上传

```
git push -u origin master

git push origin master
```

