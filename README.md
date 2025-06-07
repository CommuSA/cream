

2. **安装中间件**
   ```bash
   cd docker
   docker compose up -d mysql minio
   
3. **Minio配置**
   - 访问MinIO服务，http://localhost:19001/ 账号:admin 密码:12345678
   - 创建一个bucket，名称filedata，同时配置Access Key
   - 修改.evn.dev里的MINIO_开头的密钥消息
   
4. **初始化数据库**
   - 如果使用本地环境mysql,初始化数据时需修改源码initialize_mysql，修改数据库连接信息即可
   ```bash
     cd docker
     ./init_data.sh


5. **前端依赖安装**  
   - 前端是基于开源项目[可参考chatgpt-vue3-light-mvp安装](https://github.com/pdsuwwz/chatgpt-vue3-light-mvp)二开
   ```bash
   # 安装前端依赖&启动服务
   cd web
   
   #安装依赖
   npm install -g pnpm

   pnpm i
   
   #启动服务
   pnpm dev
   
6. **启动后端服务**
   ```bash
   #启动后端服务
   python serv.py
   ```

7. **访问服务**
 - 前端服务：http://localhost:2048


## License

[MIT](./LICENSE) License | Copyright © 2024-PRESENT [AiAdventurer](https://github.com/apconw)