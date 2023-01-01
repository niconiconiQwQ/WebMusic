<template>
  <div class="ctn-mode">
    <nav>
      <span><router-link href="#" to="/media/video">视频</router-link></span>
      <span><router-link href="#" to="/media/mv">MV</router-link></span>
    </nav>
    <router-view></router-view>
  </div>
</template>
<script setup></script>
<style lang="scss" scoped>
.ctn-mode {
  > nav {
    font-size: 1.8rem;
    span {
      margin-right: 20px;
      .router-link-active {
        font-weight: 700;
        font-size: 2rem;
        padding: 4px 0;
        border-bottom: 3px #38b2a8 solid;
      }
    }
  }
  .nav {
    width: 100%;
    height: 30px;
    margin: 20px 0px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .choice {
      position: relative;
      width: 100px;
      height: 30px;
      border: 1px solid #d9d9d9;
      border-radius: 30px;
      color: #373737;
      font-size: 14px;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      padding-left: 8px;
      .iconfont {
        font-size: 26px;
      }
      &:hover {
        background-color: #f2f2f2;
      }
    }
    .title {
      display: flex;
      li {
        color: #676767;
        padding: 2px 8px;
        cursor: pointer;
        background-color: #fdebeb;
        border-radius: 10px;
        margin-left: 20px;
        font-size: 1.2rem;
        &:hover {
          color: #000;
        }
        &.active {
        }
      }
    }
  }
  .video-box {
    > ul {
      justify-content: space-between;
      li {
        width: 24%;
        margin-bottom: 20px;
        .a-mode1 {
          height: 140px;
        }
        .name {
          color: #373737;
          text-overflow: ellipsis;
          overflow: hidden;
          white-space: nowrap;
          margin: 4px 0;
          &:hover {
            color: #000000;
          }
        }
        .creator {
          color: #e7cfcf;
        }
      }
    }
  }
}
</style>
