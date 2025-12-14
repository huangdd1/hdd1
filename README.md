[index.html](https://github.com/user-attachments/files/24151346/index.html)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>黄丹丹的草莓熊小窝</title>
    <style>
        /* 全局样式重置 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Microsoft YaHei", "幼圆", sans-serif;
        }

        /* 页面背景 */
        body {
            background-color: #FFF5F7;
            background-image: url("https://img.icons8.com/color/48/000000/teddy-bear.png");
            background-repeat: repeat;
            background-size: 70px;
            padding: 20px;
            line-height: 1.6;
        }

        /* 博客主体容器 */
        .blog-container {
            max-width: 850px;
            margin: 0 auto;
            background-color: #fff;
            border-radius: 24px;
            padding: 35px;
            box-shadow: 0 0 25px rgba(224, 119, 154, 0.3);
            border: 6px solid #F8C8DC;
        }

        /* 头部样式 */
        .blog-header {
            text-align: center;
            margin-bottom: 35px;
            background-color: #FDE6E9;
            padding: 25px;
            border-radius: 20px;
            border: 4px solid #E67E96;
        }

        .blog-header img {
            width: 160px;
            height: 160px;
            border-radius: 50%;
            border: 5px solid #FFB6C1;
            margin-bottom: 12px;
        }

        .blog-header h1 {
            color: #D6486E;
            font-size: 2.6rem;
            margin-bottom: 8px;
            text-shadow: 2px 2px 0 #FFE8F0;
        }

        .blog-header p {
            color: #8B4568;
            font-size: 1.2rem;
        }

        /* 个人信息区域 */
        .info-section {
            margin-bottom: 35px;
            background-color: #F9E8EE;
            padding: 25px;
            border-radius: 18px;
            border-left: 10px solid #E88FA8;
        }

        .info-section h2 {
            color: #A53860;
            font-size: 1.9rem;
            margin-bottom: 18px;
            border-bottom: 2px dashed #FF9AA2;
            padding-bottom: 8px;
        }

        .info-list {
            list-style: none;
            font-size: 1.2rem;
        }

        .info-list li {
            color: #4A3B40;
            padding: 8px 0;
        }

        .info-list li span {
            font-weight: bold;
            color: #C41E50;
            display: inline-block;
            width: 100px;
        }

        /* 人生格言区域 */
        .motto-section {
            margin-bottom: 35px;
            background-color: #F8E0E6;
            padding: 25px;
            border-radius: 18px;
            border-right: 10px solid #F093B0;
        }

        .motto-section h2 {
            color: #9F2B68;
            font-size: 1.9rem;
            margin-bottom: 15px;
            border-bottom: 2px dashed #B19CD9;
            padding-bottom: 8px;
        }

        .motto-content {
            font-size: 1.3rem;
            color: #5A2E48;
            text-align: center;
            padding: 15px;
            background-color: #FFF0F5;
            border-radius: 12px;
            border: 2px solid #E79FC4;
        }

        /* 分享区域 */
        .share-section {
            margin-bottom: 35px;
            background-color: #F7F0F5;
            padding: 25px;
            border-radius: 18px;
            border: 3px solid #F4B3D1;
        }

        .share-section h2 {
            color: #803B62;
            font-size: 1.9rem;
            margin-bottom: 20px;
            border-bottom: 2px dashed #FFB3C1;
            padding-bottom: 8px;
        }

        .share-item {
            background-color: #FFFBFD;
            padding: 20px;
            border-radius: 15px;
            margin-bottom: 20px;
            border-left: 6px solid #E66788;
        }

        .share-item h3 {
            color: #D13B65;
            font-size: 1.5rem;
            margin-bottom: 12px;
        }

        .share-item p {
            color: #555;
            font-size: 1.1rem;
            margin-bottom: 8px;
        }

        /* 兴趣爱好区域 */
        .hobby-section {
            margin-bottom: 35px;
            background-color: #F9F0F5;
            padding: 25px;
            border-radius: 18px;
            border: 3px solid #F1A8C5;
        }

        .hobby-section h2 {
            color: #7D2B57;
            font-size: 1.9rem;
            margin-bottom: 18px;
            border-bottom: 2px dashed #FFC2D1;
            padding-bottom: 8px;
        }

        .hobby-list {
            display: flex;
            flex-wrap: wrap;
            gap: 18px;
            margin-top: 12px;
        }

        .hobby-item {
            background-color: #FDE0E8;
            padding: 12px 25px;
            border-radius: 30px;
            border: 2px solid #E87A9C;
            font-size: 1.1rem;
            color: #8E2E57;
        }

        /* 页脚样式 */
        .blog-footer {
            text-align: center;
            margin-top: 35px;
            color: #777;
            font-size: 1.1rem;
            padding-top: 20px;
            border-top: 3px dotted #F9C5D5;
        }

        /* 响应式适配 */
        @media (max-width: 768px) {
            .blog-container {
                padding: 25px;
            }
            .blog-header h1 {
                font-size: 2.2rem;
            }
            .info-list, .hobby-item, .share-item p {
                font-size: 1rem;
            }
            .motto-content {
                font-size: 1.1rem;
            }
        }

        @media (max-width: 576px) {
            .blog-container {
                padding: 20px;
            }
            .blog-header img {
                width: 120px;
                height: 120px;
            }
            .blog-header h1 {
                font-size: 1.8rem;
            }
            .info-section h2, .motto-section h2, .share-section h2, .hobby-section h2 {
                font-size: 1.6rem;
            }
        }
    </style>
</head>
<body>
    <div class="blog-container">
        <!-- 博客头部 -->
        <div class="blog-header">
            <img src="https://img.icons8.com/fluency/96/000000/teddy-bear.png" alt="草莓熊图标">
            <h1>🍓 黄丹丹的草莓熊小窝 🍓</h1>
            <p>温柔生活，和草莓熊一起拥抱不完美～</p>
        </div>

        <!-- 个人信息区域 -->
        <div class="info-section">
            <h2>👧 关于我</h2>
            <ul class="info-list">
                <li><span>姓名：</span>黄丹丹</li>
                <li><span>性别：</span>女</li>
                <li><span>学校：</span>时珍学院</li>
                <li><span>专业：</span>数据科学与大数据技术</li>
                <li><span>班级：</span>23级大数据3班</li>
                <li><span>学号：</span>23170403037</li>
                <li><span>家乡：</span>贵州遵义正安</li>
            </ul>
        </div>

        <!-- 人生格言区域 -->
        <div class="motto-section">
            <h2>💖 我的人生格言</h2>
            <div class="motto-content">
                允许自己出错，才能活出自己
            </div>
        </div>

        <!-- 我的分享区域 -->
        <div class="share-section">
            <h2>✨ 我的小分享</h2>
            <div class="share-item">
                <h3>1. 接纳</h3>
                <p><strong>灰暗部分：</strong>原谅自己的迟钝和平庸，接受身上的不完美，就像接纳月亮有阴晴圆缺。</p>
                <p><strong>案例：</strong>作家海明威多次修改作品仍不满意，但他的创作过程本身就是文学的财富。</p>
            </div>
            <div class="share-item">
                <h3>2. 停止比较，拒绝内耗</h3>
                <p>别人的“完美人生”是他们的剧本，你的“容错人生”是你的独幕剧。</p>
            </div>
        </div>

        <!-- 兴趣爱好区域 -->
        <div class="hobby-section">
            <h2>🎨 我的兴趣爱好</h2>
            <div class="hobby-list">
                <div class="hobby-item">🎵 听歌</div>
                <div class="hobby-item">🚶 散步</div>
                <div class="hobby-item">🏸 打羽毛球</div>
                <div class="hobby-item">✂️ 做手工</div>
            </div>
        </div>

        <!-- 博客页脚 -->
        <div class="blog-footer">
            <p>🍓 草莓熊说：不完美的你，也值得被温柔对待 🍓</p>
            <p>© 2025 黄丹丹的个人博客 | 草莓熊主题</p>
        </div>
    </div>
</body>
</html>
