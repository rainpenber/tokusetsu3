# tokusetsu3-ejs
Originated form tokusetsu3 ：
The fastest way to make doujin landing page

- <https://sanographix.github.io/tokusetsu3/>


由sanographix老师的同人着陆页tumblr模板 tokusetsu3 制作的EJS模板。由于完全按照tumblr的范式编写，模板只能用于tumblr上使用。发布到自己的服务器上非常不便。我便进行了彻底的ejs重新编写。

原模板使用gulp进行打包，ejs进行模板渲染。为了尽可能的符合这一原生特性（原版本只使用ejs合并页面的三个部分header、index、footer），我将模板修改成了ejs渲染。



## Set Up / 安装

    $ npm install
    $ gulp

`/build` 以下に出力される / `/build` 得到的内容就是最终内容

原理：从根目录的`site.json`调取数据，生成`index.ejs`到`build`目录下。将`index.ejs`修改为`index.html`即可使用。
同时，请将图片文件按照原作者的要求修改为规定尺寸。可以先放在根目录的`images`目录里，gulp会自动进行压缩工作。

> 注意：由于这个作品写于好几年前，目前node已经到10的版本，gulp的语法也不太一样。请按照package.json的版本要求安装。gulp版本不要超过3.9.1
> gulp-sass请使用4.0.2版本

## 開発 / Development / 开发工作

- gh-pages 開発時、 `gh-pages` ブランチでは作業せず `gh-pages-dev` を使うこと

# License

- MIT

# Author

## Original Author
- [@sanographix](https://twitter.com/sanographix)
- <http://www.sanographix.net/>

## Ejs Modified
- [@RyanPenber](http://ryanz.cn)
- <ryanz.cn>


