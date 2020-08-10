<template>
  <div class="hello">
    <div class="head-list">
      <div class="head-content">
        <div class="head-left">
          <el-row>
            <el-col :span="3"><div class="head-l"><i class="el-icon-odometer"></i> 仪表盘</div></el-col>
            <el-col :span="3"><div class="head-l"><i class="el-icon-document"></i> 上钩列表</div></el-col>
            <el-col :span="3"><div class="head-l"><i class="el-icon-s-opportunity"></i> 分布式集群</div></el-col>
            <el-col :span="3"><div class="head-l"><i class="el-icon-message"></i> 邮件群发</div></el-col>
            <el-col :span="3"><div class="head-l"><i class="el-icon-s-tools"></i> 系统设置</div></el-col>
          </el-row>
        </div>
      </div>
    </div>
    <div class="main-content">
      <div id="title-font">
        <h3>
          仪表盘
        </h3>
        <div class="main-con">
          <el-row type="flex" class="row-bg" justify="center">
            <el-col :span="3" class="col-w ling-margin-left">
              <div class="grid-content bg-purple flex-div">
                <div class="model-con">
                  <h5 style="line-height: 12px" class="head-h">SSH</h5>
                  <p class="head-p">5</p>
                </div>
                <div class="model-con">
                  <img class="img-yangshi" src="static/img/huoyan.png" alt="">
                </div>
              </div>
            </el-col>
            <el-col :span="4" class="col-w ling-margin">
              <div class="grid-content bg-purple-light flex-div">
                <div class="model-con">
                  <h5 style="line-height: 12px" class="head-h">SSH</h5>
                  <p class="head-p">5</p>
                </div>
                <div class="model-con">
                  <img class="img-yangshi" src="static/img/huoyan.png" alt="">
                </div>
              </div>
            </el-col>
            <el-col :span="4" class="col-w ling-margin">
              <div class="grid-content bg-purple flex-div">
                <div class="model-con">
                  <h5 style="line-height: 12px" class="head-h">SSH</h5>
                  <p class="head-p">5</p>
                </div>
                <div class="model-con">
                  <img class="img-yangshi" src="static/img/huoyan.png" alt="">
                </div>
              </div>
            </el-col>
            <el-col :span="4" class="col-w ling-margin">
              <div class="grid-content bg-purple-light flex-div">
                <div class="model-con">
                  <h5 style="line-height: 12px" class="head-h">SSH</h5>
                  <p class="head-p">5</p>
                </div>
                <div class="model-con">
                  <img class="img-yangshi" src="static/img/huoyan.png" alt="">
                </div>
              </div>
            </el-col>
            <el-col :span="4" class="col-w ling-margin">
              <div class="grid-content bg-purple flex-div">
                <div class="model-con">
                  <h5 style="line-height: 12px" class="head-h">SSH</h5>
                  <p class="head-p">5</p>
                </div>
                <div class="model-con">
                  <img class="img-yangshi" src="static/img/huoyan.png" alt="">
                </div>
              </div>
            </el-col>
            <el-col :span="4" class="col-w ling-margin">
              <div class="grid-content bg-purple-light flex-div">
                <div class="model-con">
                  <h5 style="line-height: 12px" class="head-h">SSH</h5>
                  <p class="head-p">5</p>
                </div>
                <div class="model-con">
                  <img class="img-yangshi" src="static/img/huoyan.png" alt="">
                </div>
              </div>
            </el-col>
          </el-row>
          <el-row class="row-bg">
            <el-col :span="8" class="width-second mar-con">
              <div class="grid-content bg-purple-light flex-div">
                <div class="model-con">
                  <h5 style="line-height: 12px" class="head-h">SSH</h5>
                  <p class="head-p">5</p>
                </div>
                <div class="model-con">
                  <img class="img-yangshi" src="static/img/huoyan.png" alt="">
                </div>
              </div>
            </el-col>
            <el-col :span="8" class="width-second mar-con">
              <div class="grid-content bg-purple-light flex-div">
                <div class="model-con">
                  <h5 style="line-height: 12px" class="head-h">SSH</h5>
                  <p class="head-p">5</p>
                </div>
                <div class="model-con">
                  <img class="img-yangshi" src="static/img/huoyan.png" alt="">
                </div>
              </div>
            </el-col>
            <el-col :span="8" class="width-second mar-con">
              <div class="grid-content bg-purple-light flex-div">
                <div class="model-con">
                  <h5 style="line-height: 12px" class="head-h">SSH</h5>
                  <p class="head-p">5</p>
                </div>
                <div class="model-con">
                  <img class="img-yangshi" src="static/img/huoyan.png" alt="">
                </div>
              </div>
            </el-col>
            <el-col :span="8" class="width-second">
              <div class="grid-content bg-purple-light flex-div">
                <div class="model-con">
                  <h5 style="line-height: 12px" class="head-h">SSH</h5>
                  <p class="head-p">5</p>
                </div>
                <div class="model-con">
                  <img class="img-yangshi" src="static/img/huoyan.png" alt="">
                </div>
              </div>
            </el-col>
          </el-row>
        </div>
        <!--折线图-->
        <div class="zehxian">
          <div id="main-zhexian" style="width: 600px;height: 200px;" class="div-postion"></div>
        </div>
        <!-- 状态及饼图 -->
        <el-row class="foot-div">
          <el-col :span="4">
            <div class="grid-div grid-left">
              <div class="li-list">
                <div class="h-font-style">
                  <p style="">服务状态</p>
                </div>
                <div class="list-ul-div">
                  <ul>
                    <li v-for="(item,i) in listData">
                      <a href="#" class="a-font">&nbsp;{{ item }}</a>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </el-col>

          <el-col :span="10">
            <div class="grid-div grid-left">
              <div id="main" class="div-postion" style="width: 500px;height: 250px;"></div>
            </div>
          </el-col>

          <el-col :span="10">
            <div class="grid-div grid-left">
              <div id="main-ip" class="div-postion" style="width: 500px;height: 250px;"></div>
            </div>

          </el-col>
        </el-row>
      </div>
    </div>
  </div>
</template>

<script>
import echarts from 'echarts'
export default {
  name: 'Dashboard',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      listData: [
        'API',
        'PLUG',
        'WEB',
        'DEEP',
        'SSH',
        'REDIS',
        'MYSQL',
        'TELNET'
      ],
    }
  },
  mounted(){
    this.$nextTick(function() {
      this.drawPie('main');
      this.drawPieIp('main-ip');
      this.drawLine('main-zhexian')
    })
  },
  methods: {
    drawPie(id){
      this.charts = echarts.init(document.getElementById(id))
      this.charts.setOption({
        title: {
          text: '[攻击地区] TOP10',
          left: 'left'
        },
        tooltip: {
          trigger: 'item',
          formatter: '{a} <br/>{b} : {c} ({d}%)'
        },
        legend: {
          // orient: 'vertical',
          // top: 'middle',
          bottom: 10,
          left: 'center',
          data: []
        },
        series: [
          {
            type: 'pie',
            radius: '65%',
            center: ['50%', '50%'],
            selectedMode: 'single',
            data: [
              {value: 8, name: '本机地址'},
              {value: 2, name: '局域网'}
            ],
            emphasis: {
              itemStyle: {
                shadowBlur: 10,
                shadowOffsetX: 0,
                shadowColor: 'rgba(0, 0, 0, 0.5)'
              }
            }
          }
        ]
      })
    },
    drawPieIp(id){
      this.charts = echarts.init(document.getElementById(id))
      this.charts.setOption({
        title: {
          text: '[攻击IP] TOP10',
          left: 'left'
        },
        tooltip: {
          trigger: 'item',
          formatter: '{a} <br/>{b} : {c} ({d}%)'
        },
        series: [
          {
            type: 'pie',
            radius: '65%',
            center: ['50%', '50%'],
            selectedMode: 'single',
            data: [
              {value: 8, name: '127.0.0.1'},
              {value: 2, name: '192.168.0.105'}
            ],
            emphasis: {
              itemStyle: {
                shadowBlur: 10,
                shadowOffsetX: 0,
                shadowColor: 'rgba(0, 0, 0, 0.5)'
              }
            }
          }
        ]
      })
    },
    drawLine(id) {
      this.charts = echarts.init(document.getElementById(id))
      this.charts.setOption({
        title: {
          text: '最近24小时',
          left: 'left'
        },
        tooltip: {
          trigger: 'axis'
        },
        legend: {
          data: ['WEB','MYSQL']
        },
        grid: {
          left: '7%',
          right: '5%',
          bottom: '3%',
          containLabel: true
        },
        xAxis: {
          type: 'category',
          boundaryGap: false,
          data: ["10", "20", "30", "40", "50","60","70"]

        },
        yAxis: {
          type: 'value'
        },

        series: [
          {name:'WEB',type:'line',data:['10','13','45']},
          {name:'MYSQL',type:'line',data:'39'}
          ]
      })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .head-list {
    background-color: black;
    width: 100%;
    height: 60px;
    min-width: 1192px;
  }
  .main-content{
    margin: auto;
    width: 94%;
    min-width: 1192px;
  }

  .col-w{
    width: 200px;
    height: 90px;
  }

  #title-font{

  }
  .ling-margin-left{
    margin-right: 8px;
  }
  .ling-margin {
    margin-left: 8px;
    margin-right: 8px;
  }
  .bg-purple {
    background: #fff;
  }
  .bg-purple-light {
    background: #fff;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 90px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
  .width-second{
    width: 285px;
  }
  .mar-con{
    margin-right: 16px;
  }

  .head-l{
    font-family: "Andale Mono";
    font-size: 16px;
    color: #f9fafc;
  }
  .head-content{
    width: 94%;
    margin: auto;
  }
  .head-left{
    margin-left: 65px;
  }
  .head-l{
    line-height: 60px;
  }
  .model-con{
    width: 60px;
    /*background-color: red;*/
    margin-left: 8px;
    margin-right: 8px;
  }
  .flex-div{
    display: flex;
    display: -webkit-flex;
    justify-content: space-between;
    flex-direction: row;
    flex-wrap: wrap;
  }
  .head-h{
    color: gold;
  }
  .head-p{
    font-size: 20px;
    font-weight: bolder;
    line-height: 6px;
  }
  .img-yangshi{
    width: 100%;
    position: absolute;
    top: 22%;
  }
  .model-con{
    line-height: 90px;
    width: 50px;
    position: relative;
    margin: 0 14px;
  }
  .grid-div{
    height: 242px;
    background-color: white;
  }
  .grid-left{
    margin-right: 20px;
  }
  .li-list{
    margin: 0px 10px;
    /*background-color: red;*/
    width: 70%;
  }
  .h-font-style{
    height: 56px;
    width: 100px;
    line-height: 66px;
    font-weight: 800;
  }
  .foot-div{
    margin-top: 20px;
    margin-bottom: 10px;
  }
  .h-font-style h4{
    line-height: 0px;
  }
  .h-font-style p{
    font-size: 18px;
  }
  .list-ul-div{
    width: 100px;
    /*margin-left: 16px;*/
  }
  .list-ul-div ul{
    color: chartreuse;
  }
  .list-ul-div ul li{
    /*list-style-type: disc;*/
  }
  ul li::before {
    content: "● ";
    color: #0F0;
    position: relative;
    top: -1px;
    font-size: 10px;
  }
  .a-font{
    color: black;
    text-decoration:none;
    font-size: 12px;
  }
  .div-postion{
    padding-top: 16px;
  }
  .zehxian{
    width: 100%;
    margin: auto;
    height: 220px;
    background-color: #ffffff;
    margin-top: 10px;
  }
</style>
