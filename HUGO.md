### 文件结构
```txt
my-site/
├── archetypes/    模板
│   └── default.md
├── assets/
├── content/  文本内容
├── data/
├── i18n/    多语言支持
├── layouts/
├── public/       <-- created when you build your site公开
├── resources/    <-- created when you build your site静态
├── static/
├── themes/
└── hugo.toml         <-- site configuration配置文件
```

###### Step 3[](https://gohugo.io/content-management/mathematics/#step-3)

Conditionally call the partial template from the base template.模板

layouts/_default/baseof.html

```go-html-template
<head>
  ...
  {{ if .Param "math" }}
    {{ partialCached "math.html" . }}
  {{ end }}
  ...
</head>
```

The example above loads the partial template if you have set the `math` parameter in front matter to `true`. If you have not set the `math` parameter in front matter, the conditional statement falls back to the `math` parameter in your site configuration.

If you add the `$...$` delimiter pair to your configuration and JavaScript, you must double-escape the `$` when outside of math contexts, regardless of whether mathematical rendering is enabled on the page. For example: