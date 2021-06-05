# 说明

- `XDUthesis.cls`:文件修改自[StickCui/XDUthesis-personal](https://github.com/StickCui/XDUthesis-personal)，为模板文件
- `main.tex`：主文档文件
- `Figure/`:图片存放文件夹
- `ThesisFiles/`:章节、附录等文件
- `Code/`:源代码文件
-  编译方式
    ```bat
    xelatex -synctex=1 -interaction=nonstopmode main
    bibtex main
    xelatex -synctex=1 -interaction=nonstopmode main
    xelatex -synctex=1 -interaction=nonstopmode main
    ```

# 致谢

- [StickCui/XDUthesis-personal](https://github.com/StickCui/XDUthesis-personal)

