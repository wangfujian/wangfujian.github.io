---
permalink: /experimental_equipment/
title: "Experimental Equipment"
excerpt: ""
author_profile: true
---

# 实验设备

<style>
    .equipment-info {
        display: flex; /* 使用 Flexbox 布局 */
        align-items: center; /* 垂直居中对齐 */
        margin-bottom: 20px; /* 设置底部边距 */
        background-color: #fff; /* 背景颜色为白色 */
        padding: 20px; /* 内边距为20像素 */
        border-radius: 8px; /* 边框圆角半径为8像素 */
        box-shadow: 0 2px 4px rgba(0,0,0,0.1); /* 添加轻微阴影效果 */
    }

    .equipment-image {
        flex: 0 0 auto; /* 不伸缩，固定宽度 */
        margin-right: 20px; /* 右边距 */
    }

    .equipment-details {
        flex: 1; /* 伸缩，占据剩余空间 */
        text-align: justify; /* 将文本两端对齐 */
    }

    .equipment-details p {
    text-indent: 2em; /* 设置首行缩进为两个字符的宽度 */
    }

    /* 水平排列的设备信息容器样式 */
    .equipment-info.horizontal {
    flex-direction: row; /* 设置为水平排列 */
    }

    /* 垂直排列的设备信息容器样式 */
    .equipment-info.vertical {
    flex-direction: column; /* 设置为垂直排列 */
    align-items: center; /* 水平居中对齐 */
    }
    
    .equipment-image.horizontal img {
        width: 200px; /* 设置设备照片宽度 */
        height: auto; /* 自动计算高度 */
        border-radius: 8px; /* 圆角边框 */
    }

    .equipment-image.vertical img {
    width: auto; /* 设置设备照片宽度 */
    height: 300px; /* 自动计算高度 */
    border-radius: 8px; /* 圆角边框 */
    }
</style>

<div class="equipment-info horizontal">
    <div class="equipment-image horizontal">
        <img src="/images/helicopter.png" alt="设备照片">
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
        <p>如果需要了解更多关于该设备的信息，请参阅<a href="/device-document/三自由度直升机用户手册V1.2.pdf" target="_blank">设备使用手册</a>。</p>
    </div>
</div>

<div class="equipment-info horizontal">
    <div class="equipment-image horizontal">
        <img src="/images/quadrotor.png" alt="设备照片">
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
        <p>如果需要了解更多关于该设备的信息，请参阅<a href="/device-document/四旋翼飞行仿真器用户手册.pdf" target="_blank">设备使用手册</a>。</p>
    </div>
</div>

<div class="equipment-info horizontal">
    <div class="equipment-image horizontal">
        <img src="/images/balance.png" alt="设备照片">
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

<div class="equipment-info horizontal">
    <div class="equipment-image horizontal">
        <img src="/images/sanzhouyuntai.png" alt="设备照片">
    </div>
    <div class="equipment-details">
        <h2>三轴转台</h2>
        <p>三轴转台可提供高精度三自由度角位置、角速度等运动基准，模拟三自由度高动态运动环境，真实复现被测器件在不同自由度方向的运动特征，可以用于验证飞控算法、测试无人机搭载设备后飞行状态是否满足要求，大幅提升无人机及载荷的研发和测试进程并节省试飞试验时间、费用。三轴转台可以与数字模拟器联动，接收数字模拟器的信息，执行并反馈飞行模拟动作。转台上搭载的飞控、通信、光电、传感器硬件数据，在转台模拟动作同时，将数据闭环传至数字模拟平台，以支撑数字仿真与半实物仿真的闭环，具体包括：飞行控制半实物与数字模拟闭环、通信半实物与数字模拟闭环、导航定位半实物与数字模拟闭环、光电载荷半实物与数字模拟闭环。
</p>
        <p>三轴转台主要指标：</p>
        <ul>
            <li>1）转台工作方式：位置、速率、远程控制、半实物/全数字仿真。</li>
            <li>2）台面：承载能力：20kg；<br>
                        工作台面直径：300mm；<br>
                        T型台面与中框轴心线的距离：150mm；<br>
                        平面度：0.015mm；<br>
                        升降机构：升降范围0~500mm。</li>
            <li>3）轴系：倾角回转误差：±8″；<br>
                        三框转角范围：±120°；<br>
                        三轴不垂真度：±18″。</li>
            <li>4）角位置：定位精度：±8″；<br>
                        位置分辨率：2.88″；<br>
                        定位重复性：±4″。</li>
            <li>5）角速率：内框速率范围：±0.001°/s~±600°/s；<br>
                        中框速率范围：±0.001°/s~±400°/s；<br>
                        外框速率范围：±0.001°/s~±200°/s；<br>
                        三轴联动速率：60°/s；<br>
                        速率精度：1×10-4(360°平均)，1×10-3(10°平均)，1×10-2(1°平均)；<br>
                        速率平稳性：1×10-4(360°平均)，1×10-3(10°平均)，1×10-2(1°平均)；<br>
                        最大角加速度：内框±600°/s2，中框±400°/s2，外框±200°/s2。</li>
            <!-- 添加更多设备参数 -->
        </ul>
        <p>如果需要了解更多关于该设备的信息，请参阅<a href="/device-document/GHP2002型三自由度直升机实验指导书V2018.pdf" target="_blank">设备使用手册</a>。</p>
    </div>
</div>
