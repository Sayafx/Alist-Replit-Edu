# Alist-Replit-Edu
 Alist部署到replit教育版

### 安装（推荐教育版）：

创建bash语言项目

将以下代码粘贴至Replit Shell后回车

`git clone https://github.com/Sayafx/Alist-Replit-Edu.git && mv -b Alist-Replit-Edu/* ./ && mv -b Alist-Replit-Edu/.[^.]* ./ && rm -rf *~ && rm -rf Alist-Replit-Edu`

当加载完 Loading Nix environment... 后点击绿色 ▶ Run

需要自行添加数据库来保存配置

 ## Database
You may need to use another remote MySQL/Postgres database as local sqlite3 is public for everyone. Some Free MySQL/Postgres Databases:

- https://db4free.net/
- https://remotemysql.com/
- https://www.freesqldatabase.com/
- https://planetscale.com/
- https://bit.io/
- https://www.elephantsql.com/
- https://scalingo.com/
- http://cloud.yugabyte.com/

How to change the database?
> Switch to `secrets` tab then edit `System environment variables`.You can also edit raw json:
> ```json
> {
>   "DB_TYPE":"mysql",
>   "DB_HOST":"sql.com",
>   "DB_PORT":"3306",
>   "DB_USER":"alist",
>   "DB_PASS":"password",
>   "DB_NAME":"alist",
>   "DB_TABLE_PREFIX":"alist_",
>   "DB_SLL_MODE":"true"
> }
> ```
> The secrets is private so you don't need to worry about leaking your data.

## Password
The initial password is randomly generated, and you can get it by checking the console logs.
