# Hexo Theme

本主题采用 GNU GPLv3 许可证进行许可。

## 使用

请将本 repo clone 至你的 `<hexo 根目录>/themes` 文件夹。

将 `<hexo 根目录>/themes/_config-example.yml` 重命名为  `_config.yml`。

在 `<hexo 根目录>/_config.yml` 中修改：

```yaml
theme: puzzlewiki
```

即可使用。

## 主页配置

Puzzle Wiki 主页的“正在进行”与“即将开始”页面是通过配置文件生成的。在开始下列步骤前，我们非常建议您在 hexo 根目录下新建 `_config.puzzlewiki.yml`，在此配置文件进行修改以保证目录的整洁。

在配置文件中加入以下的内容：

```yaml
index:
  now: # 正在进行
    - title: # Puzzle 的标题
      image: # Puzzle 的主视觉图
      intro: # Puzzle 的简单介绍
      link: # Puzzle 对应 post 的地址
    - title: # 可增加多个 Puzzle
      image:
      intro:
      link:
  upcoming: # 尚未开始
    - title: # Puzzle 的标题
      image: # Puzzle 的主视觉图
      intro: # Puzzle 的简单介绍
      link: # Puzzle 对应 post 的地址
    - title: # 可增加多个 Puzzle
      image:
      intro:
      link:
```

即可实现主页内容的配置。如果一个分类下没有任何活动请直接把这个分类删掉以显示错误信息。