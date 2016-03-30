#MySQL Safe Update ("Dummy") Mode

```mysql --safe-updates```
or ```mysql --i-am-a-dummy```

Requires you to use unique identifiers when deleting rows, thus helping to prevent you from inadvertently emptying the table. For example, ```delete from users where 1=1``` will fail since an identifying column isn't used.

Hat Tip: This HN thread: https://news.ycombinator.com/item?id=11342968
