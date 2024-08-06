<script setup lang="ts">
import CommonButton from '../../components/CommonButton.vue'
</script>

<template>
  <div class="main">
    <div class="swiper">
      <img class="swiper-img" src="@/assets/swiper.jpg" />
      <div class="swiper-container">
        <div class="swiper-title">解锁创意新境界</div>
        <div class="swiper-title">AIGC 创作引领智绘未来</div>
        <div class="swiper-desc">利用先进AI平台，团队将 AIGC与人类创意融合</div>
        <div class="swiper-desc">为客户提供高品质的AI解决方案</div>
        <CommonButton class="swiper-btn" type="primary" :disabled="false">了解更多</CommonButton>
      </div>
    </div>
    <div class="about">
      <img class="about-img" src="@/assets/about.png" />
      <div class="about-container">
        <div class="about-title">
          <div class="about-title-left">
            <div class="about-title-left-top">
              <div class="line"></div>
              about
            </div>
            <div class="about-title-left-bottom">专注AI内容生产</div>
          </div>
          <CommonButton class="about-title-right" type="primary" :disabled="false"
            >了解更多</CommonButton
          >
        </div>
        <div class="about-desc">
          壹朵视觉成立于2024年1月18日，是一家专注于平面设计和制作领域的创新型企业。我们充分利用 AI
          大模型的强大能力，结合先进的技术平台如 Midiourney (MJ)StableDiffusion (SD) 、LoRA
          等，为客户提供独具创意和高品质的A1设计解决方案。
        </div>
        <div class="about-desc">
          我们的团队由一群富有激情和创造力的A设计师和营销人才组成。他们不仅具备深厚的设计功底和丰富的行业经验，还对
          AI 技术在设计领域的应用有着深入的研究和实践。通过不断探索和创新，我们能够将 Al
          的智能优势与人类的创意灵感完美融合,为客户打造出令人惊叹的视觉作品。
        </div>
        <div class="about-desc">
          借助 M、SD 和 LORA 等先进的 AI
          平台，我们能够大大提高设计效率，缩短项目周期同时降低成本。这些平台为我们提供了丰富的素材资源、强大的图像生成和处理能力使我们能够在短时间内为客户呈现出高质量的设计初稿，并根据客户的反馈进行快速调整和完善。
        </div>
        <div class="about-desc">
          未来，壹朵视觉将继续紧跟 AI
          技术的发展步伐，不断提升自身的技术实力和设计水平,为客户带来更多创新、优质的平面设计作品，成为推动行业发展的领军力量。
        </div>
      </div>
    </div>
    <img class="service" src="@/assets/service.png" />
    <CommonButton type="primary" :disabled="false">了解更多</CommonButton>
    <img class="case" src="@/assets/case.png" />
    <CommonButton type="primary" :disabled="false">了解更多</CommonButton>
    <img class="bottom-img" src="@/assets/bottom.png" />
    <div class="bottom">
      <div class="bottom-left">
        <div class="bottom-left-title">EXPLORE</div>
        <div class="bottom-left-items">
          <div class="bottom-left-item">HOME</div>
          <div class="bottom-left-item">CASES</div>
        </div>
      </div>
      <div class="bottom-center">
        <img class="logo" src="@/assets/logo-dark.png" />
        <div class="bottom-center-text">Welcome to our consultancy agency</div>
      </div>
      <div class="bottom-right">
        <div class="bottom-right-title">010-12345678</div>
        <div class="bottom-right-title">12345678@163.com</div>
        <div class="bottom-right-title">北京市朝阳区望京</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.main {
  width: 100vw;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.swiper {
  width: 100%;
  height: 663px;
  position: relative;
}
.swiper-img {
  position: absolute;
  width: 100%;
  height: 663px;
}
.swiper-container {
  position: absolute;
  width: 100%;
  color: #fff;
  height: 100%;
  background: linear-gradient(to right, rgba(0, 0, 0, 1), rgba(0, 0, 0, 0));
  padding-left: 150px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.swiper-title {
  font-size: 30px;
  margin-bottom: 10px;
}
.swiper-desc {
  font-size: 15px;
}
.swiper-btn {
  margin-top: 20px;
}
.about {
  width: 90%;
  display: flex;
  flex-direction: row;
  margin-top: 100px;
}
.line {
  width: 30px;
  height: 3px;
  margin-right: 6px;
  background-color: #1688f8;
}
.about-img {
  width: 40%;
}
.about-container {
  width: 50%;
}
.about-tag {
  font-size: 30px;
  color: #4c4c4c;
}
.about-title {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
.about-title-left-top {
  color: #4c4c4c;
  margin-top: 25px;
  font-size: 20px;
  display: flex;
  flex-direction: row;
  align-items: center;
}
.about-title-left-bottom {
  font-size: 30px;
  font-family: 'Times New Roman', Times, serif;
  font-weight: bolder;
  color: #000;
}
.about-desc {
  color: #4c4c4c;
  margin-top: 25px;
  font-size: 20px;
}
.service {
  margin-top: 100px;
  width: 100%;
}
.case {
  margin-top: 100px;
  width: 100%;
}
.bottom-img {
  margin-top: 80px;
  width: 100%;
  height: 140px;
}
.bottom {
  background-color: #252331;
  width: 100%;
  height: 100px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  color: #fff;
  padding-top: 10px;
}
.bottom-left {
  margin-right: 120px;
}
.bottom-left-title {
  font-size: 16px;
  margin-bottom: 10px;
}
.bottom-left-item {
  font-size: 13px;
}
.bottom-center {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: #4c4c4c;
}
.bottom-center-text {
  margin-top: 10px;
}
.bottom-right {
  margin-left: 120px;
}
.logo {
  height: 40px;
  width: 120px;
}
</style>
