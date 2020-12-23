# sqlmap-cheat-sheet

(*) It might work for all versions. 
(-) Does not apply

| TAMPER                    | MySQL         | MSSQL      | Oracle | PostgreSQL  |
|---------------------------|---------------|------------|--------|-------------|
|       apostrophemask      |       *       |      *     |    *   |      *      |
|    apostrophenullencode   |       -       |      -     |    -   |      -      |
|       appendnullbyte      |       *       |      *     |    *   |      *      |
|        base64encode       |    4,5,5.5    |    2005    |   10g  |      -      |
|          between          |      5.1      |      -     |    -   |      -      |
|          bluecoat         |       *       |      *     |    *   |      *      |
|       apostrophemask      |     9.0.3     |  2000,2005 |    -   |     9.3     |
|     charunicodeencode     | 4,5.0 and 5.5 |    2005    |   10g  | 8.3,8.4,9.0 |
|         charencode        |       *       |      -     |    -   |      -      |
|        commalessmid       |       *       |      -     |    -   |      -      |
|      concat2concatws      |       *       |      *     |    *   |      *      |
|        equaltolike        |       *       |      *     |    *   |      *      |
|          greatest         |     < 5.1     |      -     |    -   |      -      |
| halfversionedmorekeywords |  5.0 and 5.5  |      -     |    -   |      -      |
|      ifnull2ifisnull      |       *       |      *     |    *   |      *      |
|  informationschemacomment |   4,5.0,5.5   |    2005    |   10g  | 8.3,8.4,9.0 |
|         lowercase         |      5.0      |      -     |    -   |      -      |
|    modsecurityversioned   |      5.0      |      -     |    -   |      -      |
|  modsecurityzeroversioned |       *       |      *     |    *   |      *      |
|       multiplespaces      |       *       |      *     |    *   |      *      |
|  nonrecursivereplacement  |       *       |      *     |    *   |      *      |
|        overlongutf8       | 5.1.56,5.5.11 | 2000, 2005 |   N/A  |     9.0     |
|         percentage        |   4, 5.0,5.5  |    2005    |   10g  | 8.3,8.4,9.0 |
|         randomcase        |       *       |      *     |    *   |      *      |
|       randomcomments      |       *       |      *     |    *   |      *      |
|        securesphere       |   4,5.0,5.5   |    2005    |   10g  | 8.3,8.4,9.0 |
|       space2comment       |       -       |      -     |    -   |      -      |
|         space2dash        |    4.0,5.0    |      -     |    -   |      -      |
|         space2hash        |   >= 5.1.13   |      -     |    -   |      -      |
|       space2morehash      |       -       | 2000, 2005 |    -   |      -      |
|      space2mssqlblank     |       *       |      *     |    -   |      -      |
|      space2mssqlhash      |       *       |      *     |    *   |      *      |
|         space2plus        |   4,5.0,5.5   |    2005    |   10g  | 8.3,8.4,9.0 |
|     space2randomblank     |       -       |      *     |    -   |      -      |
|        sp_password        |       *       |      *     |    *   |      *      |
|      symboliclogical      |       *       |      *     |    *   |      *      |
|      unionalltounion      |       *       |      *     |    *   |      *      |
|       unmagicquotes       |   4, 5.0,5.5  |    2005    |   10g  | 8.3,8.4,9.0 |
|         uppercase         |       *       |      *     |    *   |      *      |
|          varnish          |       *       |      -     |    -   |      -      |
|     versionedkeywords     |    >=5.1.13   |      -     |    -   |      -      |
|   versionedmorekeywords   |       *       |      *     |    *   |      *      |
|       xforwardedfor       |       *       |      *     |    *   |      *      |
