<template>
  <div>
    <div class="main">
      <section class="dcr-main">
        <Perspective />
        <h1 class="title">decred china</h1>
        <div class="head">
          <img class="friends" src="../assets/frontpage_lightning.svg" />
          <div class="ontop"></div>
        </div>
        <div class="content">
          <span>
            <svg xmlns="http://www.w3.org/2000/svg" width="40" height="14" viewBox="0 0 40 14">
              <path fill="#718CA1" fill-rule="evenodd" d="M264.456055,100.172852 L263.990234,100.322266 L264.456055,100.480469 L269.834961,102.554688 L269.834961,104.277344 L262.381836,100.946289 L262.381836,99.6630859 L269.834961,96.3408203 L269.834961,98.0634766 L264.456055,100.172852 Z M277.753906,101.860352 L276.119141,101.860352 L276.119141,93.203125 L277.753906,93.203125 L277.753906,101.860352 Z M275.960938,105.147461 C275.960938,104.86621 276.044433,104.631837 276.211426,104.444336 C276.378419,104.256835 276.628905,104.163086 276.962891,104.163086 C277.296877,104.163086 277.550292,104.256835 277.723145,104.444336 C277.895997,104.631837 277.982422,104.86621 277.982422,105.147461 C277.982422,105.416994 277.895997,105.642577 277.723145,105.824219 C277.550292,106.00586 277.296877,106.09668 276.962891,106.09668 C276.628905,106.09668 276.378419,106.00586 276.211426,105.824219 C276.044433,105.642577 275.960938,105.416994 275.960938,105.147461 Z M291.130859,101.069336 L284.407227,101.069336 L284.407227,99.7333984 L291.130859,99.7333984 L291.130859,101.069336 Z M301.941406,101.069336 L295.217773,101.069336 L295.217773,99.7333984 L301.941406,99.7333984 L301.941406,101.069336 Z" transform="translate(-262 -93)"></path>
            </svg>
          </span>
          <a class="decred-china" target="_blank" href="https://github.com/decred-china">decred china</a> 是一群中国
          <a class="decred" target="_blank" href="https://decred.org">decred</a> 粉丝创建的开源组织。
          <span>
            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="9" viewBox="0 0 30 9">
              <path fill="#718CA1" fill-rule="evenodd" d="M274.928223,101.069336 L268.20459,101.069336 L268.20459,99.7333984 L274.928223,99.7333984 L274.928223,101.069336 Z M285.73877,101.069336 L279.015137,101.069336 L279.015137,99.7333984 L285.73877,99.7333984 L285.73877,101.069336 Z M289.474121,98.0107422 L289.474121,96.3320312 L297.234863,99.6542969 L297.234863,100.9375 L289.474121,104.268555 L289.474121,102.581055 L295.160645,100.436523 L295.687988,100.287109 L295.160645,100.120117 L289.474121,98.0107422 Z" transform="translate(-268 -96)"></path>
            </svg>
          </span>
        </div>
      </section>
      <section class="what">
        <h1 class="title">
          <a class="decred-china" target="_blank" href="https://github.com/decred-china">decred china</a>
          做什么
        </h1>
        <div class="logo">
          <img src="../assets/octocat.jpg" />
        </div>
        <div class="content">
          <a class="decred-china" target="_blank" href="https://github.com/decred-china">decred china</a>
          会以 <a href="https://github.com" target="_blank" class="github">Github</a> 的方式提交 Patch (Pull Request) 的方式来协助
          <a class="decred" target="_blank" href="https://decred.org">decred</a> 的代码开发，最早由
          <a target="_blank" class="detailyang" href="https://github.com/detailyang">
            detailyang (detailyang@gmail.com)
          </a>
          以开源爱好者的形式参与。
          <p>
            任何对这块有兴趣的技术或非技术同学都欢迎加入 <a href="https://github.com" target="_blank" class="github">Github</a>
            的组织，一起贡献开源的力量。
          </p>
          <p>
            目前我们维护了国内(亚洲)第一个 PoS 矿池 <a target="_blank" class="pos" href="https://pos.dcr.fans">https://pos.dcr.fans</a>，在官方的基础上做了修改，做到了同城双机房三节点高可用, 考虑到未来国内政策的原因，机房选址在阿里云的香港节点。
          </p>
          <p>
            我们也在考虑国内 PoW 的矿池，但是不同于 PoS 矿池，PoW 需要大量的算力作支撑，我们目前没有很好的算力作测试，目前该计划暂时搁浅。如果有任何人感兴趣，可以联系我们。
          </p>
        </a>
        </div>
      </section>
      <section class="decred">
        <h1>
          <a class="decred" target="_blank" href="https://decred.org">decred</a>
          是什么
        </h1>
        <div>
          <div class="desc">
            decred 是一种自主、通过混合的共识 (Pos + PoW) 系统，利益相关者可以制定规则，将其构建为去中心化、可持续和自治的货币。
          </div>
          <div class="video">
            <video style="outline:none; width:100%; height:100%;" controls>
              <source src="../assets/decred.mp4" type="video/mp4" />
            </video>
          </div>
        </div>
      </section>
    </div>
    <VFooter />
  </div>
</template>

<script>
import Perspective from "./Perspective.vue";
import Heartbeat from "./Heartbeat.vue";
import VFooter from "./VFooter.vue";

export default {
  name: 'Index',
  components: {
    Heartbeat,
    VFooter,
    Perspective,
  },
  data () {
    return {}
  }
}
</script>

<style lang="scss">
.main {
  padding-bottom: 120px;
}

section.dcr-main {
  background-image: linear-gradient(#181e24 5%,transparent 75%,transparent 100%);
  padding-bottom: 60px;
  .title {
    margin-top: -50px;
    font-size: 50px;
    font-weight: 400;
    letter-spacing: -1px;
    line-height: 58px;
    margin-bottom: 28px;
    background: -webkit-linear-gradient(#bbc1cf,#95a8c9);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .head {
    position: relative;
    -webkit-box-flex: 0;
    -webkit-flex: 0 0 auto;
    -ms-flex: 0 0 auto;
    flex: 0 0 auto;
    margin-bottom: 24px;
    .ontop {
      position: absolute;
      width: 100%;
      height: 22px;
      margin-top: -280px;
      background-image: url(../assets/empoweringemoji2x.gif);
      background-position: 50% 50%;
      background-size: auto 100%;
      background-repeat: no-repeat;
    }
    .friends {
      width: 200px;
    }
  }
  .content {
    font-size: 18px;
    font-weight: 400;
    line-height: 32px;
    color: #fff;
    background: -webkit-linear-gradient(#bbc1cf,#95a8c9);
    -webkit-background-clip: text;
  }
  .logo {
    background-color: #2971FF;
    width: 64px;
  }
}

section.what {
  background-color: #fff;
  text-align: center;
  padding-bottom: 20px;
  .title {
    padding-top: 20px;
    padding-bottom: 20px;
  }
  .logo {
    img {
      width: 200px;
    }
  }
  .content {
    width: 60%;
    margin: 0 auto;
  }
}

section.decred {
  background-color: #000;
  color: #fff;
  h1 {
    margin-top: 0px;
    padding-top: 40px;
  }
  .desc {
    margin-top: 12px;
    margin-bottom: 24px;
  }
  .video {
    width: 60%;
    margin: 0 auto;
  }
}

a.github {
  color: #41BF53;
  -webkit-text-fill-color: initial;
}

a.pos {
  color: #69D3F5;
  -webkit-text-fill-color: initial;
}

a.detailyang {
  color: #FD714A;
  -webkit-text-fill-color: initial;
}

a.decred-china {
  color: #2ED6A1;
  -webkit-text-fill-color: initial;
}

a.decred {
  color: #2971FF;
  -webkit-text-fill-color: initial;
}
</style>
