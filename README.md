# Guotong Yin - Academic Website

这是一个纯静态、无需编译的英文个人学术网站，可直接发布到 GitHub Pages。

## 首次发布

1. 登录 GitHub，新建公开仓库 `YGTong.github.io`。
2. 将本文件夹内的所有文件上传到仓库根目录。上传后应直接看到 `index.html`，不要在仓库里再套一层 `academic-website` 文件夹。
3. 打开仓库的 **Settings -> Pages**。
4. 在 **Build and deployment** 中选择 **Deploy from a branch**。
5. Branch 选择 `main`，目录选择 `/ (root)`，然后保存。
6. 等待约一两分钟，访问 `https://YGTong.github.io`。

## 发布后如何修改

最简单的方法是在 GitHub 网页中直接编辑：

1. 进入 `YGTong.github.io` 仓库。
2. 点击需要修改的文件。
3. 点击右上角铅笔按钮 **Edit this file**。
4. 修改后点击 **Commit changes**。
5. GitHub Pages 会自动重新发布，通常稍等片刻即可看到更新。

浏览器可能保留旧页面。若没有立即看到变化，可强制刷新页面：Windows 使用 `Ctrl + F5`。

## 不同内容应该修改哪里

所有文字内容都在 `index.html` 中：

- 个人简介：搜索 `Hello!`
- 研究方向：搜索 `Research interests`
- 论文成果：搜索 `Publications`
- 项目经历：搜索 `Selected projects`
- 邮箱：搜索 `yinguotong2002@xauat.edu.cn`
- GitHub 和 Scholar 链接：搜索 `profile-links`

样式位于 `styles.css`。如果只更新学术内容，通常不需要修改这个文件。

## 添加一篇新论文

在 `index.html` 的 `publication-list` 区域中，复制一个完整的 `<article class="publication"> ... </article>` 条目，然后替换年份、论文标题、作者、期刊或会议、论文链接和 BibTeX。

已发表论文使用 `data-status="published"`，审稿中论文使用 `data-status="review"`。

## 更换照片

将新照片命名为 `profile.jpg`，上传到 `assets` 文件夹并覆盖旧文件。建议使用清晰、光线自然的 JPG 照片。

如果头像裁切位置不合适，在 `index.html` 中搜索 `object-position`。第一个百分比控制左右位置，第二个百分比控制上下位置。

## 更新简历

将新简历命名为 `cv.pdf`，上传到 `assets` 文件夹并覆盖旧文件。网站中的 CV 链接不需要再次修改。

## 在电脑上批量修改

也可以把仓库下载到电脑，使用 VS Code 修改文件，再通过 GitHub Desktop 提交并推送。每次推送到 `main` 分支后，网站都会自动更新。
