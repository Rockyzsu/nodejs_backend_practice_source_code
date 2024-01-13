# node.js后端全程实战 源码
![](./resource/20230418CBEBC160.jpg)

# 勘误
* P64: 
```node.js
if(index<0){
    jsonData['uid']=1;
}
```

改成
```node.js
if(index<0){
    let key = collectName == 'users'？ 'uid':'cv_id';
    jsonData[key] = 1;
}
```