### Git 的使用

	- `Git`：分布式版本控制系统
	- 为什么要使用`Git`，便于代码管理和团队协助开发

#### Git 入门

1.  创建版本库（Repository）

   - 创建文件

   ```shell
   mkdir repository
   ```

   - 版本库下所有文件都由`Git`进行管理

   ```shell
   git init
   ```

2. 上传文件

   ```shell
   git add
   ```

3. 删除文件

   ```shell
   git rm 
   ```

4. 提交操作

   ```shell
   git commit
   ```

#### 配置`Github`远程仓库

1.  添加远程库

   ```shell
   git remote add note git@github.com:hotinL/Note.git
   ```

2. 推送服务器文件

   ```shell
   git push note master
   ```

3. 更新本地文件

   ```shell
   git pull note master
   ```


#### 注意事项

![](git使用.assets/1574740925.png)

- 无法`push`错误

  - 服务端文件发生改变,本地文件未改变,发生冲突

  - **解决方法**

    - ```shell
      # 更新文件
      git pull note master
      ```

    - ```shell
      # 推送文件
      git push note master
      ```



