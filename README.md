# Setup
1. Install `node` and `npm`

- Node

```
$ sudo apt-get update
$ sudo apt-get install nodejs
```

- Npm

```
$ sudo apt-get install npm
```

- Kiểm tra Node.js and npm đã cài đặt:

```
$ node --version
$ npm --version
```

2. Install `create-react-app`

```
$ npm install -g create-react-app
```

3. Tạo project

```
$ create-react-app my-tutorial-app
```

Nhiệm vụ của thằng này là ra 1 tạo project cùng các module như `react-script`, `react-dom`, `react`.

4. Cấu trúc của 1 project:

```
$ cd my-tutorial-app
$ ls -la
total 500
drwxrwxr-x   5 nnt142 nnt142   4096 Th11  1 14:05 .
drwxrwxr-x   5 nnt142 nnt142   4096 Th11  1 14:04 ..
-rw-rw-r--   1 nnt142 nnt142    285 Th11  1 14:05 .gitignore
drwxrwxr-x 893 nnt142 nnt142  36864 Th11  1 14:05 node_modules
-rw-rw-r--   1 nnt142 nnt142    352 Th11  1 14:05 package.json
-rw-rw-r--   1 nnt142 nnt142 336145 Th11  1 14:05 package-lock.json
drwxrwxr-x   2 nnt142 nnt142   4096 Th11  1 14:05 public
-rw-rw-r--   1 nnt142 nnt142 108875 Th11  1 14:05 README.md
drwxrwxr-x   2 nnt142 nnt142   4096 Th11  1 14:05 src
```

- File `package.json` dùng để chứa các package của Nodejs đã được cài trong project

```
$ cat package.json
{
  "name": "my-tutorial-app",
  "version": "0.1.0",
  "private": true,
  "dependencies": {
    "react": "^16.0.0",
    "react-dom": "^16.0.0",
    "react-scripts": "1.0.16"
  },
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test --env=jsdom",
    "eject": "react-scripts eject"
  }
}
```

Chạy test thử  `npm start`

Mặc định sẽ chạy ở port 3000, muốn đổi cổng sửa lại trong file package.json

```
"start": "PORT=4000 react-scripts start"
```
