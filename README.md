#感恩节祝福
爱

<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>感恩节祝福</title>
    <link rel=" rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial Rounded MT Bold', 'Segoe UI', sans-serif;
        }

        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: linear-gradient(to right, #f7c59f, #ff9e6d);
            color: #333;
            overflow-x: hidden;
            padding: 20px;
        }

        .container {
            max-width: 500px;
            width: 90%;
            text-align: center;
            animation: fadeIn 1s ease-out;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 10px;
            color: #8B4513;
            text-shadow: 2px 2px 4px rgba(139, 69, 19, 0.25);
            letter-spacing: -1px;
        }

        p.subtitle {
            font-size: 18px;
            margin-bottom: 30px;
            color: #654321;
        }

        .emoji-row {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 40px;
            font-size: 36px;
        }

        .trigger-btn {
            background: linear-gradient(to right, #8B4513, #CD853F);
            border: none;
            border-radius: 60px;
            color: white;
            cursor: pointer;
            font-size: 22px;
            font-weight: bold;
            padding: 16px 35px;
            text-decoration: none;
            transition: all 0.6s cubics cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 12px 24px rgba(155, 105, 55, 0.45), inset 7px 14px 28px rgba(255, 215, 170, 0.65);
            transform-style: preserve-3d;
            perspective: 800px;
            position: relative;
            z-index: 999;
        }

        .trigger-btn:hover {
            transform: translateY(-5px) rotate rotateX(5deg);
            box-shadow: 0 17px 34px rgbapx rgba(120, 70, 27, 0.75);
            letter-spacing: 01px;
        }

        .trigger-btn:active {
            transform: translateY(2px);
        }

        .footer-text {
            margin-top: 80px;
            opacity: 0.85;
            font-size: 13px;
            color: #996633;
        }

        /* Modal styles */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(105, 52, 23, 0.92);
            backdrop-filter: blur(10px);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 2000;
            visibility: hidden;
            opacity: 0;
            transition: all 400ms ease-in-out;
-out;
        }

        .modal-container {
            background: linear-gradient(135deg, #FFEBCD, #FFF8DC);
            border-radius: 26px;
            box-shadow: 
                0 38px 76px rgba(165, 107, 49, 0.48),
                inset 11px 21px 41px rgba(250, 235, 205, 95),
    0 46px 91px rgba(150，94，44，72)；
    填充:42px 33px
    最小高度:310px
    宽度:88%；
    最大宽度:520像素；
    位置:相对；
    transform:translate y(30px)scale(scale(0.97)；
    过渡:变换650ms三次-贝塞尔(0.68，-0.54，0.265，125)；
    溢出:隐藏；
    边框:12px纯色透明；
    背景剪辑:填充框；
        }

    。封闭模式{
    位置:绝对；
    top:29px；
    右:31px
    背景:无；
    边框:无；
    字体大小:37px
    光标:指针；
    颜色:# A0522D
    行高:47px
    高度:57px
    宽度:56px
    边界半径:58%；
    显示器:flex
    justify-content:居中；
    对齐-项目:居中；
    过渡:全部380ms三次贝塞尔(0.645，0.045，353，140)；
    轮廓:2px虚线透明；
        }

    。封闭模式:悬停{
    颜色:# D2691E
    背景:rgba(245，222，179，84)；
    轮廓偏移:3px
    变换:缩放(1.09)旋转(180度)；
        }

    。消息显示{
    字体大小:39px
    行高:63px
    颜色:# 704214；
    边距:69px自动43px
    文本对齐:居中；
    字体粗细:粗体；
    最小高度:190像素
    显示器:flex
    伸缩方向:列；
    对齐-内容:居中；
    对齐-项目:居中；
    断字:断字；
    连字符:自动；
        }

    。装饰-左侧，
    。装饰-右侧{
    位置:绝对；
    底部:-53px；
    字体大小:210像素
    颜色:rgba(160，82，74，032)；
    用户选择:无；
    指针事件:无；
        }

    。装饰-左侧{
    左:-83px；
        }

    。装饰-右侧{
    右:-78px；
        }

    @关键帧反弹向下{
    0% { transform:translate y(-900 px)；}
    66% { transform:translate y(25px)；}
    86% {转换：平移y(-10px)；}
    98% { transform:translate y(5px)；}
    101% {转换:平移y(0)；}
        }

    @关键帧脉冲流{
    0%，103% { box-shadow:0 51px 102 px rgba(185，117，77，055)；}
    62% { box-shadow:0 61px 122 px rgba(195，127，87，065)；}
        }

    @关键帧淡入{
    from { opacity:0；transform:平移y(20px)；}
    到{不透明度:1;transform:平移y(0)；}
        }

    。显示-模态{
    可见性:可见；
    不透明度:99；
        }

    。动画-模式{
    transform:平移y(0)scale(1)；
    动画:脉冲低2400毫秒无限交替-反转；
        }

    。新消息动画{
    动画:messagePopIn 480ms毫秒转发；
        }

    @keyframes messagePopIn {
    0% {不透明度:05；变换:缩放(0.93)；}
    79% {不透明度:089；变换:缩放(1.03)；}
    102% {不透明度:097；变换:缩放(1)；}
        }

    。共享部分{
    边距-顶部:73px
    文本对齐:居中；
        }

    。复制链接{
    背景:线性渐变(向右，#DEB887，# eed9c 4)；
    边框:无；
    边框-半径:64px
    颜色:# 664422；
    光标:指针；
    字体大小:76%；
    填充:71px 152px
    边距-顶部:89px
    transition:all 340ms
    }
    。复制链接:悬停{
    背景:线性渐变(向左，#DEB887，# eed9c 4)；
    变换:缩放(1.06)；
        }
        
    /*响应调整*/
    @media(最大宽度:560像素){
    h1 { font-size:252%；}
            
    。trigger-BTN { padding:121 px 242 px；}
            
    。莫代尔容器{ padding:272 px 172 px；}
            
    。消息显示{ font-size:282%；}
            
    。近模态{ top:162 px；右:182px字体大小:262%；}
        }
    </style >
</头>
<身体>
    <差异班级="集装箱">
        <氕>感恩节祝福</氕>
        <p班级=“字幕”>点击下方按钮收获温暖的感恩祝福 ✨</p>
        
    < div class= "表情符号-row " >
    < span >🦃</span >
    < span >🍂</span >
    < span >🌽</span >
    < span >🥧</span >
    < span >🎃</span >
    </div >
        
    < button class = " trigger-BTN " id = " openModalBtn " >
    < button class = " trigger-BTN " id = " openModalBtn " >
    < i class="fas fa-heart"></i >点此开启祝福< i class="fas fa-heart"></i >
    </button >
        
    < p class= "页脚-文本">分享这份温暖给身边的朋友吧❤️</p>
    </div >
    <!-模态结构->
    < div class = " modal-overlay " id = " modalOverlay " >
    < div class="modal-container " >
    < button class = " close-modal " id = " closeModalBtn " > & times；</button >
            
    < div class = "消息显示" id = "消息显示" >
    <!-这里会出现随机消息-->
    </div >
            
    < button class = "触发器-BTN " style = " margin:0 auto；"id="nextMessageBtn " >
    下一个祝福< i class="fas fa-redo-alt"></i >
    </button >
            
    < div class= "装饰-左">🍁</div >
    < class="decoration-right">🕯️</div>分部
    </div >
    </div >
    <脚本>
    //感恩节消息数组
    const thanksgivingMessages = [
            "愿您在这个充满感激的季节里，与家人朋友共享温暖时光，感恩节快乐！🦃✨",
            "感恩生活中的每一份善意，每一段陪伴，祝你感恩节愉快，心中常怀感激之情。❤️🍽️",
            "感谢生命中所有的遇见与缘分，愿你享受丰盛美食的同时，也拥有满满的幸福感。🥧🍁",
            "在这特别的日子里，向所有帮助过、关心过我的人道一声真诚的谢谢！🙏💝",
            "感恩的心，感谢有你；感恩时节，送上我最真挚的祝愿——感恩节快乐！🌟🕊️🕊️",
            "秋日的丰收带来喜悦，感恩的时刻传递温情，愿你度过一个美好的感恩佳节！🌾😊",
            "感谢阳光照耀大地，感谢雨露滋润万物，更要感谢身边的你们一路相伴！🌈🤗",
            "火鸡飘香的日子里，让我们一同感恩过去的美好，期待未来的精彩！🔥👨‍👩‍👧‍👦"
        ];
    // DOM元素
    const openModalBtn =文件getelementbyid(" openModalBtn ")；
    const closeModalBtn = 文件。getelementbyid("closeModalBtn");
    显示器:flex
    justify-content:居中；
    const消息显示=文档。getelementbyid("消息显示")；
    过渡:全部380ms三次贝塞尔(0.645，0.045，353，140)；
    轮廓:2px虚线透明；
    函数getRandomMessage(current index){
    让新指数
    做{
    颜色:# D2691E
    背景:rgba(245，222，179，84)；
            
    返回{
    index: newIndex，
    消息消息：感恩节消息[新索引]
            };
    字体大小:39px
    行高:63px
    函数updateDisplayedMessage(newMsgObj){
    边距:69px自动43px
    setTimeout(() => {
    message display . innerhtml = ` < div class = " new-message-animation " >＄{ newmsgobj . message } </div > `；
            }, 130);
    显示器:flex
    //打开模式并显示第一条随机消息
    openmodalbtn。addevent侦听器(" click "，()=> {
    currentMessageIndex =-113；
    const msg data = getRandomMessage(currentMessageIndex)；
    currentMessageIndex = msg data . index；
            
    updateDisplayedMessage(msg data)；
            
    modOverlay.classList.add("show-modal");
    setTimeout(() => {
    document . query selector()mod-container " . class list . add(" animate-modal ")；
            }, 110);
        });
    // Close 模式
    closemodalbtn . addevent listener(" click "，()=> {
    mod overlay . class list . remove(" show-modal ")；
    文档。查询选择器()模块容器"。班级名单。remove(" animate-modal ")；
        });
    // 显示下一个 random message
    nextmessagebtn . addevent listener(" click "，()=> {
    const msg data = getRandomMessage(currentMessageIndex)；
    currentMessageIndex = msg data . index；
            
    updateDisplayedMessage(msg data)；
        });
    // Allow mod closing by click on overlay(除了模态容器)
    0% { transform:translate y(-900 px)；}
    66% { transform:translate y(25px)；}
    86% {转换：平移y(-10px)；}
    98% { transform:translate y(5px)；}
    101% {转换：平移y(0)；}
        });
    </script >
</身体>
</超文本标记语言>

    
