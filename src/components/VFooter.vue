<template>
  <div class="footer">
    <footer style="background-color: -webkit-linear-gradient(#bbc1cf,#95a8c9);">
      <div class="qrcode">
        <a class="community" target="_blank" href="https://github.com/decred-china">
          <img class="github" width="480" src="../assets/github.png" alt="github">
          <icon name="github"></icon>
        </a>
<!--       <a class="community" target="_blank" href="https://t.me/etherpush">
        <img class="telegram" width="480" src="../assets/telegram.png" alt="telegram">
        <icon name="telegram"></icon>
      </a> -->
<!--       <a class="community" target="_blank" href="https://twitter.com/etherpush">
        <img class="twitter" width="480" src="../assets/etherpush-twitter.png" alt="twitter">
        <icon name="twitter"></icon>
      </a> -->
      <a class="community" target="_blank" href="https://u.wechat.com/MPSWL4PbElyPQ9HMaRZLm6E">
        <img width="480" src="../assets/wechat.png" alt="wechat">
        <icon name="wechat"></icon>
      </a>
      <a class="community" target="_blank" href="//shang.qq.com/wpa/qunwpa?idkey=9ccecd9b52fa4645cf2368eaee6cc4ad8ad39df2b9da4bd7f259ca6edf808b27">
        <img width="480" src="../assets/qq.png" alt="qq">
        <icon name="qq"></icon>
      </a>
      <a class="community" target="_blank" href="https://pos.dcr.fans">
        <img width="480" src="../assets/pos.png" alt="qq">
        <span style="font-size:8px;">PoS</span>
      </a>
      <a class="community" target="_blank" href="https://dcr66.com">
        <img width="480" src="../assets/bbs.png" alt="qq">
        <span style="font-size:8px;">论坛</span>
      </a>
    </div>
      <p class="copyright">
        <a class="decred-china" target="_blank" href="https://github.com/decred-china">decred-china</a>
        由
        <a target="_blank" class="detailyang" href="https://github.com/detailyang">
          detailyang (detailyang@gmail.com)
        </a>
        维护
        <Heartbeat />
      </p>
    </footer>
  </div>
</template>

<script>
import Heartbeat from "./Heartbeat.vue";

export default {
  components: {
    Heartbeat,
  },
  data() {
    return {};
  }
}
</script>

<style lang="scss" scoped>
.footer {
  display: flex;
  -ms-flex-align: center;
  align-items: center;
  -ms-flex-pack: center;
  justify-content: center;
  padding-top: 10px;
  padding-bottom: 10px;
  width: 100%;
  background-color: rgba(39,48,56,.94);
  position: relative;
  display: -ms-flexbox;
  display: flex;
  padding: 16px 0;
  -ms-flex-align: center;
  align-items: center;
  position: fixed;
  bottom: 0;
  left: 0;
  z-index: 1000;
  border-top: 1px solid #383b44;
  p.copyright {
    font-size: 14px;
    font-weight: 400;
    line-height: 32px;
    background: -webkit-linear-gradient(#bbc1cf,#95a8c9);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .qrcode {
    a {
      color: #fff;
    }

    a.community {
        position: relative;
    }

    .community img {
      position: absolute;
      z-index: 99;
      top: -135px;
      right: -28px;
      width: 7.5rem;
      max-width: none;
      height: 7.5rem;
      transform: scale(0);
      transform-origin: top right;
      opacity: 0;
      box-shadow: 0px 0px 30px 10px rgba(90, 82, 255, 0.49);
      transition: box-shadow .2s ease-in-out;
      -moz-transition: box-shadow .2s ease-in-out;
      -webkit-transition: box-shadow .2s ease-in-out;
    }

    .community:hover img {
        transform: scale(1);
        opacity: 1;
    }

    .fa-icon {
      width: 2em;
    }
  }
}

</style>
