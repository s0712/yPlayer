<template>
    <div class="home">
        <header>
            <p>
                <input type="text">
                <span>搜索</span>
            </p>
            <p>
                热门搜索: <a href="">沙漠骆驼</a><a href="">沙漠骆驼</a><a href="">沙漠骆驼</a><a href="">沙漠骆驼</a><a href="">沙漠骆驼</a>
            </p>
        </header>
        <main>
            <!-- title -->
            <section class="t">
                <img src="../../../static/bg/head.jpg"
                     alt="">
                <div>
                    <p><span>毛不易</span>
                        <span>单曲127</span>
                        <span>专辑12</span>
                        <span>MV70</span></p>
                    <span>>播放歌手热门歌曲</span>
                </div>
            </section>
            <!-- nav -->
            <section class="nav">
                <span>单曲</span>
                <span>专辑</span>
                <span>MV</span>
                <span>歌单</span>
                <span>用户</span>
                <span>歌词</span>
            </section>
            <!-- main -->
            <section class="m">
                <div class="m_btns">
                    <span>>播放全部</span>
                    <span>>添加到</span>
                    <span>>下载</span>
                    <span>>批量操作</span>
                </div>
            </section>
        </main>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.home{
    background-color: #fafafa;
     header{
        background: url('../../../static/bg/bg_search.jpg');
        height: 247px;
        display: flex;
       flex-direction: column;
        p{
            width: 100%;
            text-align: center;
        }
        p:first-child{
                margin-top: 104px;
        }
        p:last-child{
            margin-top: 15px;
            color: #fff;
            font-size: 14px;
            a{
            color: #fff;
            font-size: 14px;
            margin-right: 20px;
            }
        }
  }
  main{
      border:1px solid red;
        width: 1200px;
        margin: 0 auto;
        .t{
            border:1px solid blue;
            display: flex;
            margin: 20px 0;
            >img{
                height: 96px;
                width: 96px;
                border-radius: 50%;
                margin-right: 20px;
            }
            >div{
                display: flex;
                flex-direction: column;
                justify-content: center;
                >p{
                    line-height: 40px;
                    span{
                        margin-right: 30px;
                    }
                }
                >span{
                    border: 1px solid #31c27c;
                    background-color: #31c27c;
                    width: 179px;
                    height:38px;
                    line-height: 38px;
                    text-align: center;
                    color: #fff;
                    border-radius: 2px;
                    font-size: 14px
                }
            }
        }
        .nav{
            height: 56px;
            line-height: 56px;
            margin-bottom: 30px;
            span{
                margin-right: 55px;
            }
        }
        .m{
            &_btns{
                span{
                    min-width: 122px;
                    text-align: center;
                    border: 1px solid #c9c9c9;
                    border-radius: 2px;
                    font-size: 14px;
                    margin-right: 6px;
                    padding: 0 23px;
                    height: 38px;
                    line-height: 38px;
                    display: inline-block;
                    white-space: nowrap;
                    box-sizing: border-box;
                    overflow: hidden;
                    cursor: pointer;
                }
                   
            }
        }
  }
}
</style>
