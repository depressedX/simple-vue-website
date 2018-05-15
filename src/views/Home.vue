<template>
    <div class="home">
        <the-nav-bar id="nav-bar"/>
        <slider id="banner-slider" :displayedItems="testItems"/>
        <section class="section section-news">
            <div class="section__title">
                <h1 class="section__title__eng">NEWS</h1>
                <h1 class="section__title__chs">新闻通告</h1>
            </div>
            <my-hr/>
            <div class="section-news__content section__content" style="display: flex;justify-content: space-between">
                <preview-box
                        title="动态"
                        title-eng="Events"
                        all-link="baidu.com"
                >
                    <news-display-box
                            box-class-name="news-box"
                            :date="Date.now()"
                            title="为“海洋山东”扬帆领航——山东大学服务海洋山东纪实"
                            :background-image="newsSamplePic1"
                    />
                    <news-display-box
                            box-class-name="news-box"
                            :date="Date.now()"
                            title="经济强省建设中的“山大智慧”——山东大学服务山东经济强省建设纪实"
                            :background-image="newsSamplePic2"
                    />
                </preview-box>
                <preview-box
                        title="通知"
                        title-eng="Notices"
                        all-link="baidu.com"
                        style="width: 300px">
                    <notice-item
                            title="test"
                            :date="Date.now()"
                            style="margin: .5em 0"/>
                    <notice-item
                            title="test"
                            :date="Date.now()"
                            style="margin: .5em 0"/>
                    <notice-item
                            title="test"
                            :date="Date.now()"
                            style="margin: .5em 0"/>
                    <notice-item
                            title="test"
                            :date="Date.now()"
                            style="margin: .5em 0"/>
                    <notice-item
                            title="test"
                            :date="Date.now()"
                            style="margin: .5em 0"/>
                    <notice-item
                            title="test"
                            :date="Date.now()"
                            style="margin: .5em 0"/>
                    <notice-item
                            title="关于推荐新材料领域专家的函(鲁经 信字（2017）186号)"
                            :date="Date.now()"
                            style="margin: .5em 0"/>
                </preview-box>
            </div>
        </section>
        <section class="section section-experts">
            <div class="section__title">
                <h1 class="section__title__eng">EXPERTS</h1>
                <h1 class="section__title__chs">专家资源</h1>
            </div>
            <div class="section-experts__content section__content">
                <div class="expert-group">
                    <expert-display-box
                            :profile="experts1"
                            name="李树忱"
                            introduction="土建与水利学院副院长，现任地下工程系教授、博士生导师。担任中国岩石力学与工程学会地下工程分会..."
                    />
                    <expert-display-box
                            :profile="experts1"
                            name="李树忱"
                            introduction="土建与水利学院副院长，现任地下工程系教授、博士生导师。担任中国岩石力学与工程学会地下工程分会..."
                    />
                    <expert-display-box
                            :profile="experts1"
                            name="李树忱"
                            introduction="土建与水利学院副院长，现任地下工程系教授、博士生导师。担任中国岩石力学与工程学会地下工程分会..."
                    />
                    <expert-display-box
                            :profile="experts1"
                            name="李树忱"
                            introduction="土建与水利学院副院长，现任地下工程系教授、博士生导师。担任中国岩石力学与工程学会地下工程分会..."
                    />
                </div>
                <div class="more">
                    <blue-button>更多专家资源</blue-button>
                </div>
            </div>
        </section>
        <section class="section section-research">
            <div class="section__title">
                <h1 class="section__title__eng">REASEARCH</h1>
                <h1 class="section__title__chs">研究专利</h1>
            </div>
            <my-hr/>
            <div class="section-research__content section__content">
                <el-menu
                        class="research-nav-bar"
                        mode="horizontal"
                >
                    <el-menu-item index="1">技术成果</el-menu-item>
                    <el-menu-item index="2">专利信息</el-menu-item>
                    <el-menu-item index="3">成功案例</el-menu-item>
                </el-menu>
                <div class="research-display-box-wrapper" style="font-size: .9em">
                    <research-display-box
                            :photo="research1"
                            title="电子信息类"
                            title-eng="digital information"
                            content="万兆网络多核处理器SOC芯片产业化"
                    />
                    <research-display-box
                            :photo="research1"
                            title="电子信息类"
                            title-eng="digital information"
                            content="万兆网络多核处理器SOC芯片产业化"
                    />
                    <research-display-box
                            :photo="research1"
                            title="电子信息类"
                            title-eng="digital information"
                            content="万兆网络多核处理器SOC芯片产业化"
                    />
                </div>
                <div class="more">
                    <blue-button>更多技术成果</blue-button>
                </div>
            </div>
        </section>
        <footer class="section section-footer">
            <div class="section__content section-footer__content">
                <div class="left">
                    <div class="row row-1">
                        <div class="left">
                            <img src="../assets/logo2.png" class="logo">
                            <div class="info">
                                <p>地 址：山东济南山大南路27号明德楼B410房间 B435房间</p>
                                <p>邮 编：250100</p>
                                <p>传 真：0531-88362065 </p>
                                <p>Email：jszy@sdu.edu.cn </p>
                            </div>
                        </div>
                        <div class="right friendly-link">
                            <h1>友情链接</h1>
                            <P>
                                教育部科技发展中心<br/>
                                山东省科技厅<br/>
                                山东省经济和信息化委员会<br/>
                                山东省科技成果转化服务平台<br/>
                                山东政产学研合作联盟<br/>
                                山东省科学院<br/>
                                山东大学国家大学科技园<br/>
                                海尔集团<br>
                                山东大学科学技术研究院
                            </p>
                        </div>
                    </div>
                    <div class="row row-2 copyright">
                        CopyRight © 2014-2016 All Rights Reserved By The Technology Transfer Center of Shandong University
                    </div>
                </div>
                <div class="right contact">
                    <h1>中心工作事务联系方式</h1>
                    <div class="contact__content">
                        <div class="left">
                            <h2>知识产权运营</h2>
                            <p>联系人：丁茹<br/>
                                办公地址：中心校区明德楼B区410房间<br/>
                                办公电话：0531-88362680
                            </p>
                            <h2>中心综合事务管理</h2>
                            <p>联系人：孙岩<br/>
                                办公地址：中心校区明德楼B区410房间<br/>
                                办公电话：0531-88362680
                            </p>
                            <h2>对外合作</h2>
                            <p>联系人：徐阳<br/>
                                办公地址：中心校区明德楼B区410房间<br/>
                                办公电话：0531-88362686
                            </p>
                        </div>
                        <div class="right">
                            <p>
                                联系人：刘灿刚<br/>
                                办公地址：中心校区明德楼B区410房间<br/>
                                办公电话：0531-88392972</p>
                            <p>联系人：孙海磊<br/>
                                办公地址：中心校区明德楼B区410房间<br/>
                                办公电话：0531-88392972</p>
                            <p>联系人：朱西民<br/>
                                办公地址：中心校区明德楼B区435房间<br/>
                                办公电话：0531-88369600</p>
                            <p>联系人：柳瞳瞳<br/>
                                办公地址：中心校区明德楼B区435房间<br/>
                                办公电话：0531-88369600
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </footer>
        <the-footer/>
    </div>
</template>

<script>
    import pic1 from '../assets/bb3.jpg'
    import pic2 from '../assets/bb2.jpg'
    import research1 from '../assets/research_1.jpg'
    import experts1 from '../assets/experts_1.jpg'
    import TheNavBar from '../components/TheNavBar'
    import Slider from '../components/Slider'
    import MyHr from "../components/MyHr";
    import PreviewBox from "../components/PreviewBox";
    import NewsDisplayBox from "../components/NewsDisplayBox";

    import newsSamplePic1 from '../assets/news_sample1.jpg'
    import newsSamplePic2 from '../assets/news_sample2.jpg'
    import NoticeItem from "../components/NoticeItem";
    import ExpertDisplayBox from "../components/ExpertDisplayBox";
    import BlueButton from "../components/BlueButton";
    import ResearchDisplayBox from "../components/ResearchDisplayBox";
    import TheFooter from "../components/TheFooter";

    export default {
        name: 'home',
        components: {
            TheFooter,
            ResearchDisplayBox,
            BlueButton, ExpertDisplayBox, NoticeItem, NewsDisplayBox, PreviewBox, MyHr, TheNavBar, Slider
        },
        data() {
            return {
                testItems: [
                    {
                        title: 'test1',
                        subTitle: 'test2',
                        backgroundImage: pic1
                    },
                    {
                        title: 'test1',
                        subTitle: 'test2',
                        backgroundImage: pic2
                    }
                ],
                newsSamplePic1,
                newsSamplePic2,
                experts1,
                research1
            }
        }
    }
</script>
<style scoped>
    #nav-bar {
        position: absolute;
        left: 0;
        top: 0;
        z-index: 999;

    }

    #banner-slider {
        width: 100%;
        height: 500px;
    }

    /*section类表示主页中的某一栏 有统一的padding*/
    .section {
        padding: 2em 4em 4em 4em;
    }

    .section__content {
        padding: 4em 0;
    }

    .section__title {
        text-align: center;
        margin-bottom: 2em;
    }

    .section__title__eng {
        margin: 0;
        font-size: 2.5em;
        color: rgb(202, 202, 202);
    }

    .section__title__chs {
        font-weight: normal;
        margin: 0;
        font-size: 1.3em;
        color: rgb(20, 68, 131);
    }

    .news-box {
        display: inline-block;
        margin: 0 2em;
    }

    .section-experts {
        background-image: url("../assets/bg_experts.jpg");
        background-size: cover;
    }

    .section-experts__content {
    }

    .section-experts__content .expert-group {
        padding: 0 2em 3em 2em;
        display: flex;
        justify-content: space-between;
        flex-wrap: nowrap;
    }

    .section__content .more {
        padding-bottom: 1em;
        font-size: .9em;
        text-align: center;
    }

    .research-nav-bar {
        padding-left: 400px;
        margin-bottom: 4em;
    }

    .research-display-box-wrapper {
        font-size: .9em;
        display: flex;
        flex-wrap: nowrap;
        justify-content: space-between;
        padding: 0 2em 3em 2em;
    }


    @import "../style/footer.css";
</style>
