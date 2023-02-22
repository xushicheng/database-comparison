# 对比前端数据库的性能

## 使用方法

pnpm install 然后就可以跑起来

## 1000 条数据测试结果

| 数据库 | 耗时(毫秒) |
| ---- | ---- |
| loki | 7 |
| idb | 18 |
| 原生indexedDB | 75 |
| dexie 单条插入 | 170 |
| dexie 批量插入 | 130 |
| localForage | 5415 |

## 1万条数据测试结果

| 数据库 | 耗时(毫秒) |
| ---- | ---- |
| loki | 13 |
| idb | 172 |
| 原生indexedDB | 753 |
| dexie 单条插入 | 1036 |
| dexie 批量插入 | 945 |
| localForage | 两分钟还没返回, 不考虑 |

## 10万条数据测试结果

| 数据库 | 耗时(毫秒) |
| ---- | ---- |
| loki | 272 |
| idb | 5334 |
| 原生indexedDB | 8687 |
| dexie | 10464 |
| dexie 批量插入 | 10816 |
| localForage | 两分钟还没返回, 不考虑 |
