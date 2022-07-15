# Alist-Replit-Edu
 Alist部署到replit教育版

### 安装（推荐教育版）：

将以下代码粘贴至Replit Shell后回车

`git clone https://github.com/Sayafx/typechonreplit.git && mv -b typechonreplit/* ./ && mv -b typechonreplit/.[^.]* ./ && rm -rf *~ && rm -rf typechonreplit`

当加载完 Detected change in environment, reloading shell...
在Shell输入`sh main.sh`初始化，初始化完成后点击绿色 ▶ Run 运行


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
