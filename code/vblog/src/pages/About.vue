<template>
<Layout>
    <section>
        <div style="min-height: 600px;" class="">
            <div class="el-card is-never-shadow">
                <!---->
                <div class="el-card__body">
                    <div style="" class="markdown-body">
                        <h1>VBlog</h1>
                        <p><img src="https://img.shields.io/github/languages/top/github-laziji/VBlog.svg?style=flat" alt=""><br>
                            <img src="https://img.shields.io/github/stars/gitHub-laziji/VBlog.svg?style=social" alt=""></p>
                        <h2>目录</h2>
                        <ul>
                            <li><a href="#%E7%AE%80%E4%BB%8B" target="_blank">简介</a></li>
                            <li><a href="#%E6%BC%94%E7%A4%BA%E5%9C%B0%E5%9D%80" target="_blank">演示地址</a></li>
                            <li><a href="#%E9%A1%B9%E7%9B%AE%E6%BA%90%E7%A0%81" target="_blank">项目源码</a></li>
                            <li><a href="#%E9%A1%B9%E7%9B%AE%E7%89%B9%E7%82%B9" target="_blank">项目特点</a></li>
                            <li><a href="#%E6%9B%B4%E6%96%B0%E8%AE%B0%E5%BD%95" target="_blank">更新记录</a></li>
                            <li><a href="#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8" target="_blank">快速使用</a></li>
                        </ul>
                        <h2>简介</h2>
                        <p>博客可搭建在 GitHub Pages 上,<br>
                            文章数据储存于gist 中, 通过Github API 与数据进行交互, 实现无后台、可动态发布文章的博客系统</p>
                        <blockquote>
                            <p>最近暂无更新计划</p>
                        </blockquote>
                        <h2>演示地址</h2>
                        <p><a href="https://github-laziji.github.io" target="_blank">https://github-laziji.github.io</a></p>
                        <h2>项目源码</h2>
                        <p><a href="https://github.com/GitHub-Laziji/vblog" target="_blank">https://github.com/GitHub-Laziji/vblog</a></p>
                        <h2>项目特点</h2>
                        <ul>
                            <li>[x] 基于 GitHub Pages 无需服务器</li>
                            <li>[x] 改进传统 GitHub Pages 不能动态发布的缺陷</li>
                            <li>[x] 包含电脑端和移动端</li>
                            <li>[x] 单页面应用</li>
                        </ul>
                        <h2>更新记录</h2>
                        <h4>2018.5.19 更新</h4>
                        <ul>
                            <li>增加使用帮助页面</li>
                            <li>修复没有README.md时候出现的BUG</li>
                        </ul>
                        <h4>2018.5.16 更新</h4>
                        <ul>
                            <li>显示粉丝数量</li>
                            <li>增加粉丝详情页面</li>
                        </ul>
                        <h4>2018.5.15 更新</h4>
                        <ul>
                            <li>粉丝页面优化没有粉丝的情况</li>
                            <li>修改有的图片越界</li>
                            <li>配置增加是否自动播放音乐</li>
                            <li>去除默认音乐</li>
                        </ul>
                        <h4>2018.5.13 更新</h4>
                        <ul>
                            <li>电脑端增加社交圈, 查看粉丝和关注的用户</li>
                        </ul>
                        <h4>2018.5.11 更新</h4>
                        <ul>
                            <li>移动端增加博客, 项目, 个人中心, 移动端和PC端共用API, 页面独立</li>
                            <li>修复文章样式奇怪的BUG</li>
                        </ul>
                        <h4>2018.5.8 更新</h4>
                        <ul>
                            <li>增加配置选项</li>
                            <li>改善富文本编辑器</li>
                        </ul>
                        <h4>2018.5.6 更新</h4>
                        <ul>
                            <li>状态栏增加音乐播放器</li>
                        </ul>
                        <h4>2018.5.5 更新</h4>
                        <ul>
                            <li>增加了系统配置, 可以动态修改标题, 描述, 背景等配置</li>
                        </ul>
                        <h4>2018.5.2 更新</h4>
                        <ul>
                            <li>增加博客和项目列表的分页</li>
                            <li>增加分享链接</li>
                            <li>改进Token绑定验证</li>
                            <li>修改代码结构</li>
                        </ul>
                        <h4>2018.4.30 更新</h4>
                        <ul>
                            <li>添加了从github获取个人开源项目的功能,显示信息更加全面,显示开源项目列表</li>
                            <li>Readme 从github动态获取</li>
                        </ul>
                        <h4>2018.4.29 更新</h4>
                        <ul>
                            <li>增加个人信息的状态栏</li>
                            <li>修复发图片博文的BUG</li>
                        </ul>
                        <h2>快速使用</h2>
                        <p>搭建博客只需2步</p>
                        <ul>
                            <li>点击github头像旁边的 “+” 号 选择 <code>Import repository</code>克隆地址填 <code>https://github.com/GitHub-Laziji/GitHub-Laziji.github.io</code>项目名填 <code>你的用户名.github.io</code></li>
                            <li>克隆完成后 修改文件 <code>/static/configuration.json</code> 中的 <code>githubUsername</code> 为自己的github用户名</li>
                        </ul>
                        <p>类似演示地址其中 GitHub-Laziji 为我的用户名</p>
                        <p>现在 <code>https://你的用户名.github.io</code> 就是你的个人博客了,例如<a href="https://github-laziji.github.io" target="_blank">https://github-laziji.github.io</a></p>
                        <h4>获取Token</h4>
                        <p>在 <code>github &gt; settings &gt; Developer settings &gt; Personal access tokens</code> 勾选<code>gist</code> 和 <code>repo</code>权限 获取<code>Token</code></p>
                        <hr>
                        <p>作者 <em>Laziji</em></p>
                    </div>
                </div>
            </div>
            <div class="el-loading-mask" style="display: none;">
                <div class="el-loading-spinner"><svg viewBox="25 25 50 50" class="circular">
                        <circle cx="50" cy="50" r="20" fill="none" class="path"></circle>
                    </svg>
                    <!---->
                </div>
            </div>
        </div>
    </section>
</Layout>
</template>

<script>
export default {
    metaInfo: {
        title: 'About us'
    }
}
</script>
