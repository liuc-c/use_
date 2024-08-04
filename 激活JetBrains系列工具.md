# 激活JetBrains系列工具

## 激活流程

1. 打开热心大佬网站传送门[JETBRA.IN CHECKER | IPFS](https://3.jetbra.in/)。

   > 当热佬的网站被显示欺诈、码不能复制、网站被墙时，可自行部署热佬网站，具体操作参见 [热佬网站部署](#热佬网站部署)。

2. 通过传送门网站进入热佬网站后，在页面上方提示框中下载`jetbra.zip`文件。

3. 解压下载的`jetbra.zip`文件，进入`\vmoptions`目录下。

4. 修改所有`.vmoptions`文件，在文件中添加以下2句内容，使工具使用`UTF-8`作为默认编码。

   ```json
   -Dfile.encoding=UTF-8
   -Dconsole.encoding=UTF-8
   ```

5. 修改完成后，返回上级目录，进入`\scripts`目录下，双击`install-current-user.vbs`运行文件。

   > Mac OS or Linux: 执行`install.sh`文件
   > Windows:
   >
   > - `install-current-user.vbs` (只对当前用户生效)
   > - `install-all-users.vbs` (对所有用户生效)

6. 运行文件后，等待弹窗提示`done`时表示配置完成。

7. 打开JetBrains系列任意工具，从热佬网站复制对应工具的激活码，填写激活码激活即可。

   > 如果已经登陆了JetBrains账号，则需先退出账号再进行激活码激活



## 热佬网站部署

1. 有自己的域名，解析托管在[Cloudflare](https://dash.cloudflare.com/)，这个自己完成不解释。
2. 点开自己解析在`Cloudflare`的域名，在左侧菜单栏最后找到`Web3`菜单。
3. 点开`Web3`菜单，订阅免费的`IPFS DNSLink Gateway`，免费就够用。
4. 订阅成功后，单击`创建网关`按钮，开始创建。
   - `主机名`填写你要的完整域名，比如：`jb.zhile.io`。
   - `网关描述`这个可选，爱填不填。
   - `网关类型`选择`IPFS DNSLink`。
   - 最后一个`内容路径`填写：`/ipns/3.jetbra.in`。
   - 点击`部署`按钮进行部署。
5. 部署完大约等`1分钟`生效，这个地址就能访问了。