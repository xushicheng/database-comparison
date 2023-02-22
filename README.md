# 对比前端数据库的性能

## 使用方法

pnpm install 然后就可以跑起来

## 1万条数据测试结果

loki 13ms
idb 172ms
原生indexedDB  753ms
dexie 972ms
localForage 两分钟还没返回, 不考虑

## 10万条数据测试结果

loki 272ms
idb 5334ms
原生indexedDB  8687ms
dexie 10464ms
localForage 两分钟还没返回, 不考虑
