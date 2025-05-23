
| Name |                                          |                     |                   |          | Value                                                      |
| :--: | :--------------------------------------: | :-----------------: | :---------------: | :------- | :--------------------------------------------------------- |
| URL  |                                          |                     |                   |          | `https://user:pw@keepass.info:80/path/example.php?q=e&s=t` |
|      |            Schema / Protocol             |                     |                   |          | `https`                                                    |
|      | HierarchicalPart / HierPart / RMV Schema |                     |                   |          | `user:pw@keepass.info:80/path/example.php?q=e&s=t`         |
|      |                                          |      Authority      |                   |          | `user:pw@keepass.info:80`                                  |
|      |                                          |                     |     UserInfo      |          | `user:pw`                                                  |
|      |                                          |                     |                   | Username | `user`                                                     |
|      |                                          |                     |                   | Password | `pw`                                                       |
|      |                                          |                     | Host / DomainName |          | `keepass.info`                                             |
|      |                                          |                     |       Port        |          | `80`                                                       |
|      |                                          |        Path         |                   |          | `/path/example.php`                                        |
|      |                                          | Query / QueryString |                   |          | `?q=e&s=t`                                                 |
|      |                                          |                     |       Key1        |          | q                                                          |
|      |                                          |                     |      Value1       |          | e                                                          |
|      |                                          |                     |       Key2        |          | s                                                          |
|      |                                          |                     |      Value2       |          | t                                                          |