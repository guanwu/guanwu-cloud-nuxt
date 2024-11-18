<template>
    <div class="container">
        <!-- 基本信息 -->
        <div class="card">
            <h3>基本信息</h3>
            <div class="info-section">
                <!-- 第一行 -->
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">境内发货人</el-text>
                    <input type="text" id="a1" value="上海威盛报关有限公司"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">出境关别</el-text>
                    <input type="text" id="a2" value="上海海关"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">备案号</el-text>
                    <input type="text" id="a3" value="JITTLLSE3"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">出口日期</el-text>
                    <input type="text" id="a4" placeholder="自动生成"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">申报日期</el-text>
                    <input type="text" id="a5" placeholder="自动生成"></input>
                </div>

                <!-- 第二行 -->
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">境外收货人</el-text>
                    <input type="text" id="a6" value="NO"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">运输方式</el-text>
                    <input type="text" id="a7" value="水路运输"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">运输工具</el-text>
                    <input type="text" id="a8" value="AU9389"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">航次号</el-text>
                    <input type="text" id="a9" value="//"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">提运单号</el-text>
                    <input type="text" id="a10" value="D893NH_8938930RR"></input>
                </div>

                <!-- 第三行 -->
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">生产销售单位</el-text>
                    <input type="text" id="a11" value="上海威盛报关有限公司"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">监管方式</el-text>
                    <input type="text" id="a12" value="一般贸易"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">征免性质</el-text>
                    <input type="text" id="a13" value="一般征税"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">许可证号</el-text>
                    <input type="text" id="a14" value="JI-FO-ERHG93"></input>
                </div>

                <!-- 第四行 -->
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">合同协议号</el-text>
                    <input type="text" id="a15" value="FF-24023902"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">贸易国地</el-text>
                    <input type="text" id="a16" value="中国"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">运抵国地</el-text>
                    <input type="text" id="a17" value="日本"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">指运港</el-text>
                    <input type="text" id="a18" value="上海洋山"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">离境口岸</el-text>
                    <input type="text" id="a19" value="上海洋山"></input>
                </div>

                <!-- 第五行 -->
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">包装种类</el-text>
                    <input type="text" id="a20" value="天然木托"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">其他包装</el-text>
                    <input type="text" id="a21" value="散装,裸装"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">件数</el-text>
                    <input type="text" id="a22" value="100"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">净重（千克）</el-text>
                    <input type="text" id="a23" value="100.00"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">毛重（千克）</el-text>
                    <input type="text" id="a24" value="102.00"></input>
                </div>

                <!-- 第六行 -->
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">成交方式</el-text>
                    <input type="text" id="a25" value="CIF"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">运费</el-text>
                    <input type="text" id="a26" value="$1200.00"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">保费</el-text>
                    <input type="text" id="a27" value="$400.00"></input>
                </div>
                <div class="info-item quarter-width">
                    <el-text class="mx-1" type="info">杂费</el-text>
                    <input type="text" id="a29" value="$0.00"></input>
                </div>

                <!-- 第八行 -->
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">特殊关系确认</el-text>
                    <input type="text" id="a30" value="是"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">价格影响确认</el-text>
                    <input type="text" id="a30" value="是"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">特许权使用费确认</el-text>
                    <input type="text" id="a31" value="是"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">公式定价确认</el-text>
                    <input type="text" id="a32" value="是"></input>
                </div>
                <div class="info-item eighth-width">
                    <el-text class="mx-1" type="info">暂定价格确认</el-text>
                    <input type="text" id="a33" value="是"></input>
                </div>

                <!-- 第七行 -->
                <div class="info-item full-width">
                    <el-text class="mx-1" type="info">标记唛码及备注</el-text>
                    <input type="text" id="a34" value="N/M"></input>
                </div>

            </div>
        </div>
    </div>
</template>

<style scoped>
* {
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background-color: #f3f3f3;
    margin: 0;
    padding: 20px;
}

.container {
    width: 90%;
    max-width: 1200px;
    min-width: 800px;
    margin: auto;
}

.card {
    background-color: #fff;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    margin-bottom: 20px;
    padding: 20px;
}

h3 {
    margin: 0 0 20px;
    font-size: 18px;
    font-weight: bold;
}

.info-section {
    display: flex;
    flex-wrap: wrap;
    border: 1px solid #ddd;
    border-radius: 8px;
}

.info-item {
    padding: 5px;
    font-size: 14px;
    border-bottom: 1px solid #ddd;
    transition: background-color 0.3s ease;
}

/* 去掉最后一行的下边框 */
.info-item:nth-last-child(-n+1) {
    border-bottom: none;
}

/* 鼠标悬停时背景变为淡绿色 */
.info-item:hover {
    background-color: #e6f7e6;
}

.info-item label {
    display: block;
    color: #888;
    font-size: 13px;
}

.info-item input {
    border: none;
    background-color: transparent;
    cursor: default;
    color: #333;
    width: 100%;
    padding: 2px 0;
    font-size: 14px;
}

.info-item input:focus {
    outline: none;
}

/* 自定义每个输入框的宽度比例 */
.full-width {
    flex: 1 1 100%;
}

.half-width {
    flex: 1 1 50%;
}

.quarter-width {
    flex: 1 1 25%;
}

.eighth-width {
    flex: 1 1 12.5%;
}
</style>