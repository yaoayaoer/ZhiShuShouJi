# 数据库设计

## ER 图

```mermaid
erDiagram
    USER[用户] ||--o{ USER_BOOK[用户书架] : 拥有
    BOOK[书籍] ||--o{ USER_BOOK : 加入
    USER_BOOK ||--o{ READING_RECORD[阅读记录] : 产生
    USER_BOOK ||--o{ NOTE[笔记] : 包含
    USER ||--o{ TAG[标签] : 创建
    NOTE ||--o{ NOTE_TAG[笔记标签关联] : 关联
    TAG ||--o{ NOTE_TAG : 关联
```
