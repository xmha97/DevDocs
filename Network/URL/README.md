# Uniform Resource Identifier (URI)

| Name |                             |                     |                   |          | Value                                                          |
| :--: | :-------------------------: | :-----------------: | :---------------: | :------- | :------------------------------------------------------------- |
| URL  |                             |                     |                   |          | `https://user:pw@example.com:80/path/example.php?q=e&s=t#nose` |
|      |      Schema / Protocol      |                     |                   |          | `https`                                                        |
|      | HierarchicalPart / HierPart |                     |                   |          | `user:pw@example.com:80/path/example.php?q=e&s=t`              |
|      |                             |      Authority      |                   |          | `user:pw@example.com:80`                                       |
|      |                             |                     |     UserInfo      |          | `user:pw`                                                      |
|      |                             |                     |                   | Username | `user`                                                         |
|      |                             |                     |                   | Password | `pw`                                                           |
|      |                             |                     | Host / DomainName |          | `example.com`                                                  |
|      |                             |                     |       Port        |          | `80`                                                           |
|      |                             |        Path         |                   |          | `/path/example.php`                                            |
|      |                             | Query / QueryString |                   |          | `?q=e&s=t`                                                     |
|      |                             |                     |       Key1        |          | q                                                              |
|      |                             |                     |      Value1       |          | e                                                              |
|      |                             |                     |       Key2        |          | s                                                              |
|      |                             |                     |      Value2       |          | t                                                              |
|      |          Fragment           |                     |                   |          | nose                                                           |