---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>


# 🏠 Introduction
太仓飞控实验室是一个致力于航空航天领域研究与开发的实验室。我们的实验室汇集了一群热爱航空航天科技的年轻科研人员，专注于无人机、卫星技术、飞行控制系统等领域的研究与创新。在太仓飞控实验室，我们秉承着创新、合作和实践的理念。我们的团队包括工程师、研究人员和学生，共同致力于解决航空航天领域的关键问题。我们注重理论与实践相结合，通过开展实验和项目，培养团队成员的实际操作能力和解决问题的技能。实验室的研究方向涵盖了多个领域，包括但不限于飞行控制系统设计、导航与定位技术、飞行器动力学建模与仿真、无人机应用开发等。我们鼓励团队成员在这些领域中探索创新思路，提出新的理论和方法，推动航空航天科技的发展。太仓飞控实验室致力于搭建国际化的合作平台，与国内外相关高校、科研机构和企业建立合作关系，共同开展科研项目，促进技术交流与合作。如果你对航空航天领域充满激情，并希望在一个充满创新和挑战的环境中发展自己，欢迎加入太仓飞控实验室，与我们一起探索未来的航空航天世界！

<a href='https://www.nwpu.edu.cn/' style='text-decoration: none;'><strong>点击</strong><span id='total_cit'>加入我们！</span></a>



# 👨‍🎓 Teachers
<style>
    .teacher-info {
        display: flex; /* 使用 Flexbox 布局 */
        align-items: center; /* 垂直居中对齐 */
        margin-bottom: 20px; /* 设置底部边距 */
    }

    .teacher-image {
        flex: 0 0 auto; /* 不伸缩，固定宽度 */
        margin-right: 20px; /* 右边距 */
    }

    .teacher-details {
        flex: 1; /* 伸缩，占据剩余空间 */
    }

    .teacher-image img {
        width: 150px; /* 设置照片宽度 */
        height: auto; /* 自动计算高度 */
        border-radius: 50%; /* 圆形边框 */
    }
</style>

<div class="teacher-info">
    <div class="teacher-image">
        <img src="images/dangqingqing.png" alt="教师照片">
    </div>
    <div class="teacher-details">
        <h2>党庆庆</h2>
        <p>学历：博士研究生毕业</p>
        <p>性别：男</p>
        <p>学位：工学博士学位</p>
        <p>学院：民航学院</p>
        <p>职称：中级</p>
        <p>电子邮箱：dangqingqing@nwpu.edu.cn</p>
    </div>
</div>

<div class="teacher-info">
    <div class="teacher-image">
        <img src="images/chenjianlin.png" alt="教师照片">
    </div>
    <div class="teacher-details">
        <h2>陈建林</h2>
        <p>学历：博士研究生毕业</p>
        <p>性别：男</p>
        <p>学位：工学博士学位</p>
        <p>学院：民航学院</p>
        <p>职称：副高</p>
        <p>电子邮箱：jianlin.chen@nwpu.edu.cn</p>
    </div>
</div>


# 🛠️ Experimental Equipment 
<style>
    .equipment-info {
        display: flex; /* 使用 Flexbox 布局 */
        align-items: center; /* 垂直居中对齐 */
        margin-bottom: 20px; /* 设置底部边距 */
    }

    .equipment-image {
        flex: 0 0 auto; /* 不伸缩，固定宽度 */
        margin-right: 20px; /* 右边距 */
    }

    .equipment-details {
        flex: 1; /* 伸缩，占据剩余空间 */
    }

    .equipment-image img {
        width: 150px; /* 设置设备照片宽度 */
        height: auto; /* 自动计算高度 */
        border-radius: 8px; /* 圆角边框 */
    }
</style>

<div class="equipment-info">
    <div class="equipment-image">
        <img src="helicopter.png" alt="设备照片">
    </div>
    <div class="equipment-details">
        <h2>三自由度直升机</h2>
        <p>三自由度直升机是一款非常有趣的教学产品，学生可以把控制直升机飞行姿态和速度算法运用到该平台上，来实际验证算法的控制效果。从PID、LQR、H∞到模糊控制算法都可在此平台上试验，适用于自动化、机电一体化和航空航天等相关专业。</p>
        <p>实验内容：</p>
        <ul>
            <li>1：动力学数学模型；</li>
            <li>2：系统分析；</li>
            <li>3：线性二次型最优调节；</li>
            <li>4：LQR调节器的仿真与实现；</li>
            <li>5：系统误差分析。</li>
            <!-- 添加更多设备参数 -->
        </ul>
    </div>
</div>

<div class="equipment-info">
    <div class="equipment-image">
        <img src="quadrotor.png" alt="设备照片">
    </div>
    <div class="equipment-details">
        <h2>四旋翼飞行仿真器</h2>
        <p>四旋翼飞行仿真器是四输入三输出的系统。四输入分别为前、后、左、右四个电机的电压;三输出分别为俯仰角、滚动角、偏航角。所以可以选用现代控制理论的状态反馈或者LQR线性二次型最优控制理论设计调节器，通过实验不仅可以学习状态反馈和LQR控制的设计应用 方法，而且可以比较不同状态时系统性能指标的变化，来比较状态反馈和LQR控制之间区别联系。
        四旋翼飞行仿真器本体由安装在万向节轴杆上的四个带螺旋桨的电机提供动力。其中，前、左和右三个电机实现本体的俯仰姿态，左右两个电机实现飞本体的滚动姿态，后电机实现本体的偏航姿态。通过安装在平台上的三个编码器检测飞本体的三种姿态，反馈入控制器计算出控制量，控制电机转动，以此来实现本体的俯仰、偏航和滚动三种姿态的精确定位。</p>
        <p>实验内容：</p>
        <ul>
            <li>1：动力学分析；</li>
            <li>2：建立状态方程；</li>
            <li>3：线性二次型最优调节器；</li>
            <li>4：LQR调节器的阶跃仿真；</li>
            <li>5：四旋翼LQR六状态阶跃响应测试；</li>
            <li>6：四旋翼LQR九状态阶跃响应测试；</li>
            <li>7：系统误差分析。</li>
            <!-- 添加更多设备参数 -->
        </ul>
    </div>
</div>

<div class="equipment-info">
    <div class="equipment-image">
        <img src="balance.png" alt="设备照片">
    </div>
    <div class="equipment-details">
        <h2>自平衡小车</h2>
        <p>自平衡小车是一个自由移动的三自由度倒立摆系统，可以实现本体前后移动、前后俯仰、左右转向偏航三种运动模式。小车上的倾角计和两个编码器能实时反馈电机的转角和俯仰偏角进入控制器，从而控制左右两轮的力矩使小车保持平衡，并可以通过无线遥控控制小车。</p>
        <p>实验内容：</p>
        <ul>
            <li>1：直线一级倒立摆及数学模型；</li>
            <li>2：线性二次型最优调节器；</li>
            <li>3：自平衡小车的数学模型建立 ；</li>
            <li>4：LQR线性二次型最优调节器的设计；</li>
            <li>5：自平衡小车的LQR调节器Matlab仿真设计；</li>
            <li>6：自平衡小车的状态反馈Matlab仿真设计。</li>
            <!-- 添加更多设备参数 -->
        </ul>
    </div>
</div>

# 🎖 Honors and Awards
- *2021.10* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.09* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 

# 📖 Educations
- *2019.06 - 2022.04 (now)*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2015.09 - 2019.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 

# 💬 Invited Talks
- *2021.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/)

# 💻 Internships
- *2019.05 - 2020.02*, [Lorem](https://github.com/), China.
