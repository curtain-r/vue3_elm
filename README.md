### 1. 如何控制一个前端项目的编码规范

使用`.editorconfig` 文件来规定一个项目中的文件的规范，比如本项目
```javascript
// .editorconfig
# EditorConfig is awesome: https://EditorConfig.org

# top-most EditorConfig file
root = true

# Unix-style newlines with a newline ending every file
[*]
end_of_line = lf
insert_final_newline = true

# Matches multiple files with brace expansion notation
# Set default charset
[*.{vue, js}]
charset = utf-8

# 4 space indentation
[*.vue]
indent_style = tab
indent_size = 2


# Indentation override for all JS under lib directory
[*.js]
indent_style = tab
indent_size = 2

# Matches the exact files either package.json or .travis.yml
[{package.json,.travis.yml}]
indent_style = space
indent_size = 2
```