# 删除外键约束
Syntax
```

```
Example
```
#先查看外键约束名称
show create table tableName;
#删除
alter table rbac_role_authority drop foreign key constraintName;
```

# 添加外键约束
Synatx
```$xslt

```
Example
```
alter table rbac_role_authority  add constraint rbac_role_authority_ibfk_1
  foreign key (roleid) references opsmanager.rbac_role (id) on delete cascade on update cascade;

alter table rbac_role_authority  add constraint rbac_role_authority_ibfk_2
  foreign key (authorityid) references opsmanager.rbac_authority (id) on delete cascade on update cascade;
```

# 