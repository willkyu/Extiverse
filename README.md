# 扩展市场

本仓库用于供应扩展文件内容和对应的接口

## 牌堆
### 目录结构
```
├─deck
│  ├─作者
│  │  ├─classic
│  │  │  ├─__index.json
│  │  │  ├─牌堆1.json
│  │  │  ├─牌堆2.json
│  │  │  └─...
│  │  └─resource
│  └─...
└─...
```


#### 作者空间
每一个作者可以在`deck`目录下以自己的名字直接创建一整个目录，所有的有关作品的操作都可以在自己的目录内完成。  

#### 类型牌堆
目前支持了`classic`牌堆，这是最基础的`json`格式牌堆，可以在自己的作者空间内创建对应的目录，并将对应的牌堆放入该目录。  

#### 索引文件
特别的，名为`__index.json`的文件不会被当作牌堆，而是用于描述当前目录下的牌堆的附加信息，例如`牌堆名`、`作者`、`描述`、`版本号`等等，这些信息将被用于生成扩展市场的接口数据，并最终展示在用户与扩展市场的应用界面上。  
其基本格式如下：  
```json
{
    "明日方舟-Arknights(单抽-十连).json": {
        "name": "明日方舟",
        "version": "201111",
        "version_code": 1,
        "desc": "明日方舟干员寻访，干员档案数据全部来自ArknightsWiKi，文案版权属于鹰角网络。在这里，你甚至可以抽出绝版暴行",
        "author": "lunzhiPenxil"
    },
    "明日方舟卡池-Arknight(卡池-[对应卡池名称]).json": {
        "name": "明日方舟卡池",
        "version": "201111",
        "version_code": 1,
        "desc": "明日方舟卡池寻访，干员档案数据全部来自ArknightsWiKi，文案版权属于鹰角网络。在这里，你甚至可以抽出绝版暴行",
        "author": "lunzhiPenxil"
    }
}
```

## 提交的途径
通常来说，在`Github`上我们以`Pull Request（拉取请求）`的方式来提交自己的改动，得益于`Github`完善的设计，整个提交过程你完全可以图形化的完成。
