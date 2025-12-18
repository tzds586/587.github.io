[个人简历.HTML](https://github.com/user-attachments/files/24232461/default.HTML)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>王梓峰睿的简历</title>
    <style>
        /* 全局样式重置与基础设置 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box; /* 盒模型优化，避免宽高受内边距影响 */
        }

        body {
            font-family: "Microsoft YaHei", sans-serif;
            line-height: 1.6;
            background-color: #f5f5f5;
            padding: 20px;
        }

        /* 栅格布局容器：核心栅格设置 */
        .grid-container {
            display: grid;
            /* 定义列：移动端1列，桌面端（768px以上）12列（经典栅格列数） */
            grid-template-columns: repeat(12, 1fr);
            /* 栅格间距（行、列之间的空隙） */
            gap: 20px;
            /* 最大宽度限制，居中显示 */
            max-width: 1200px;
            margin: 0 auto;
        }

        /* 栅格项：占满12列（全宽） */
        .grid-col-12 {
            grid-column: span 12;
        }

        /* 栅格项：占6列（半宽），仅桌面端生效 */
        @media (min-width: 768px) {
            .grid-col-6 {
                grid-column: span 6;
            }
        }

        /* 导航栏样式 */
        .nav {
            background-color: #fff;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            text-align: center;
        }

        .nav a {
            text-decoration: none;
            color: #333;
            margin: 0 15px;
            font-size: 18px;
        }

        .nav a:hover {
            color: #0066cc;
        }

        .nav .back-to-top {
            float: right;
        }

        /* 媒体元素容器样式 */
        .media-container {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            /* 媒体元素内部也用栅格布局，实现音频和视频的并排/堆叠 */
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            align-items: center;
        }

        /* 内容区域样式 */
        .content-section {
            background-color: #ffffffc6;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }

        /* 图片样式 */
        .photo {
            width: 100%;
            max-width: 200px;
            height: auto; /* 自适应高度，保持比例 */
            border: 2px solid #000;
            margin-bottom: 20px;
        }

        /* 滚动文字区域 */
        marquee {
            width: 100%;
            height: 400px;
            bgcolor: rgb(173, 230, 219);
            direction: up;
            behavior: alternate;
            scrollamount: 10;
            scrolldelay: 100;
            loop: infinite;
        }

        /* 清除浮动 */
        .clearfix::after {
            content: "";
            display: table;
            clear: both;
        }
    </style>
</head>
<body>
    <!-- 栅格布局容器：所有内容都放在这个容器内 -->
    <div class="grid-container">
        <!-- 导航栏：占满12列 -->
        <div class="grid-col-12 nav">
            <a href="#个人简历">个人简历</a>
            <a href="#获奖经历">获奖经历</a>
            <a href="#个人爱好">个人爱好</a>
            <a href="#在读学校">在读学校</a>
            <a href="#顶部" class="back-to-top">回到顶部</a>
        </div>

        <!-- 顶部锚点 -->
        <a name="顶部"></a>

        <!-- 媒体区域：占满12列 -->
        <div class="grid-col-12 media-container">
            <!-- 音频元素 -->
            <audio src="792498676.mp3" controls loop muted preload="metadata">
                您的浏览器不支持音频元素。
            </audio>

            <!-- 视频元素 -->
            <video src="9d6b433bacbb93c998d6a77f331ded38.mp4" controls width="100%" max-width="400px" height="auto" poster="20200618112410_tobrq.gif" preload="auto" loop muted>
                您的浏览器不支持视频元素。
            </video>
        </div>

        <!-- 个人简历：桌面端占12列，移动端也占12列（可根据需求调整为6列） -->
        <div class="grid-col-12 content-section clearfix" id="个人简历">
            <h3>个人简历 <a href="#顶部" style="font-size: 14px; text-decoration: none;">回到顶部</a></h3>
            <!-- 图片及映射 -->
            <img src="OIP-C (1).jpg" title="王梓峰睿的照片" alt="王梓峰睿" 
                 class="photo" usemap="#photoMap">
            <map name="photoMap">
                <area shape="circle" coords="150,50,50" href="http://www.baidu.com" target="_blank" alt="百度链接">
                <area shape="circle" coords="10,190,10" href="http://www.360.com" target="_blank" alt="360链接">
            </map>

            <!-- 滚动文字区域 -->
            <marquee onmouseover="this.stop()" onmouseout="this.start()">
                <p>王梓峰睿，男，19岁</p>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem odit, inventore quaerat aliquid, provident veritatis illo reprehenderit ipsa est repudiandae consectetur laborum, optio omnis sunt officia quisquam. Consectetur, accusantium exercitationem.</p>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem odit, inventore quaerat aliquid, provident veritatis illo reprehenderit ipsa est repudiandae consectetur laborum, optio omnis sunt officia quisquam. Consectetur, accusantium exercitationem.</p>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem odit, inventore quaerat aliquid, provident veritatis illo reprehenderit ipsa est repudiandae consectetur laborum, optio omnis sunt officia quisquam. Consectetur, accusantium exercitationem.</p>
            </marquee>
        </div>

        <!-- 获奖经历：桌面端可拆分为6列，这里先占12列，可根据需求调整 -->
        <div class="grid-col-12 content-section" id="获奖经历">
            <h3>获奖经历 <a href="#顶部" style="font-size: 14px; text-decoration: none;">回到顶部</a></h3>
            <p>三好学生，四好少年（小学）</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem odit, inventore quaerat aliquid, provident veritatis illo reprehenderit ipsa est repudiandae consectetur laborum, optio omnis sunt officia quisquam. Consectetur, accusantium exercitationem.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem odit, inventore quaerat aliquid, provident veritatis illo reprehenderit ipsa est repudiandae consectetur laborum, optio omnis sunt officia quisquam. Consectetur, accusantium exercitationem.</p>
        </div>

        <!-- 个人爱好：可与在读学校并排（桌面端各占6列） -->
        <div class="grid-col-12 grid-col-6 content-section" id="个人爱好">
            <h3>个人爱好 <a href="#顶部" style="font-size: 14px; text-decoration: none;">回到顶部</a></h3>
            <p>打游戏，吃，睡觉</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem odit, inventore quaerat aliquid, provident veritatis illo reprehenderit ipsa est repudiandae consectetur laborum, optio omnis sunt officia quisquam. Consectetur, accusantium exercitationem.</p>
        </div>

        <!-- 在读学校：桌面端占6列，与个人爱好并排 -->
        <div class="grid-col-12 grid-col-6 content-section" id="在读学校">
            <h3>在读学校 <a href="#顶部" style="font-size: 14px; text-decoration: none;">回到顶部</a></h3>
            <p>大连海洋大学</p>
            <p><a href="https://www.dlou.edu.cn/" target="_blank">学校官网</a></p>
        </div>
    </div>
</body>
</html>
