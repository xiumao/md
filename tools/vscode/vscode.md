### 配置宏命令 行尾自动加分号

- 第一步
> 文件 C:\Users\Administrator\AppData\Roaming\Code\User\settings.json
```md
"macros": {
        "end_semicolon": [ // 末尾加分号
            "cursorLineEnd",
            {
                "command": "type",
                "args": {
                    "text": ";"
                }
            },
        ]
    }
```

- 第二步
> 文件 C:\Users\Administrator\AppData\Roaming\Code\User\keybindings.json
```md
{
    "key": "ctrl+Enter",
    "command": "macros.end_semicolon"   
}
```