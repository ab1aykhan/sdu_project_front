<template>
  <div class="login">
    <div class="login__inner">
      <div class="login__item login__left">
        <svg xmlns="http://www.w3.org/2000/svg" width="180" height="230" viewBox="0 0 120 136" fill="none">
          <g filter="url(#filter0_d_1_4)">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M113.694 26.8303L57.6247 57.7583C56.7503 58.2406 55.6568 58.2725 54.7493 57.8422L14.8844 38.9405C12.9629 38.0294 10.648 39.2673 10.628 41.2166L10.3978 63.7213C10.3879 64.6919 10.9812 65.5867 11.9368 66.0423L54.7428 86.4531C55.6537 86.8874 56.7532 86.8552 57.6305 86.3685L108.062 58.3908C109.994 57.3187 112.489 58.5653 112.489 60.6033V95.5844C112.489 96.4892 111.964 97.329 111.105 97.8021L57.6401 127.215C56.7573 127.701 55.6529 127.728 54.7423 127.286L12.1915 106.624C11.2551 106.169 10.6718 105.291 10.6718 104.336V103.985C10.6718 102.019 13.0086 100.764 14.941 101.691L54.7432 120.79C55.6537 121.227 56.7545 121.197 57.6335 120.711L104.728 94.6808C105.585 94.2072 106.107 93.3689 106.107 92.466V67.589C106.107 65.5481 106.495 65.4483 104.563 66.5264L57.6558 93.1141C56.7651 93.6111 55.6447 93.638 54.7256 93.1846L5.50284 68.9039C4.5759 68.4467 4 67.5731 4 66.6243V36.3129C4 35.4109 4.52095 34.5733 5.37667 34.0993L65.5273 0.786048C66.406 0.299381 67.507 0.268439 68.4179 0.704808L113.541 22.3195C115.517 23.2658 115.602 25.778 113.694 26.8303ZM104.656 25.2358L66.9466 6.76423L19.374 33.7096L56.2137 51.5122L104.656 25.2358Z" fill="#0B1E71"/>
          <path d="M53.8886 103.737L14.2777 84.8495C12.4701 83.9876 10.3817 85.3055 10.3817 87.3081C10.3817 88.345 10.9705 89.292 11.9004 89.7508L53.8587 110.448C55.3332 111.175 57.0711 111.131 58.5068 110.33L95.626 89.62C96.545 89.1073 97.1145 88.1374 97.1145 87.0851C97.1145 84.8725 94.7382 83.4733 92.8034 84.5467L58.4662 103.596C57.0528 104.38 55.3476 104.433 53.8886 103.737Z" fill="#5BB1F9"/>
          <path d="M58.4662 67.7213L100.377 44.988C102.308 43.9407 104.657 45.3387 104.657 47.5354C104.657 48.591 104.083 49.563 103.158 50.0729L58.4565 74.7304C57.0484 75.5071 55.3525 75.5591 53.8994 74.8701L21.2634 59.3959C20.1096 58.8489 19.3741 57.6861 19.3741 56.4092C19.3741 53.9713 21.9229 52.3722 24.1179 53.4329L53.9067 67.8282C55.3552 68.5282 57.052 68.4884 58.4662 67.7213Z" fill="#5BB1F9"/>
          </g>
          <defs>
          <filter id="filter0_d_1_4" x="0" y="0.394409" width="119.075" height="135.209" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
          <feFlood flood-opacity="0" result="BackgroundImageFix"/>
          <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
          <feOffset dy="4"/>
          <feGaussianBlur stdDeviation="2"/>
          <feComposite in2="hardAlpha" operator="out"/>
          <feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"/>
          <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow_1_4"/>
          <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow_1_4" result="shape"/>
          </filter>
          </defs>
        </svg>
      </div>
      <div class="login__item login__right">
        <div class="login__header">
          <h3 class="login__title">Welcome to Spotutor</h3>
          <div class="login__create-account">Don't have a account? <a href="#" class="login__link">Create</a></div> 
        </div>
        <div class="login__form">
          <el-form
            :label-position="'top'"
          >
            <el-form-item label="E-mail"
                          class="login__input"
            >
              <el-input size="large" 
                placeholder="example@stu.sdu.edu.kz" 
              />
            </el-form-item>
            <el-form-item label="Password"
                          class="login__input"
            >
              <el-input size="large" 
                placeholder="6+ Character, 1 Capital letter" 
              />
            </el-form-item>
            <el-form-item>
              <el-button type="primary" class="login__btn">Sign in</el-button>
            </el-form-item>
          </el-form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .login{
    height:100%;
    width: 100%;
    &__inner{
      height:100%;
      width: 100%;
      display: flex;
    }
    &__item{
      flex: 1;
    }
    &__left{
      background-color: #FAFBFC;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    &__right{
      display: flex;
      padding: 30px;
      flex-direction:column;
    }
    &__header{
      margin-bottom: 30px;
    }
    &__title{
      font-size: 34px;
      margin: 0 0 20px 0;
    }
    &__create-account{
      color:#C1C2C7
    }
    &__btn{
      width: 100%;
      padding: 20px 0;
      font-size: 18px;
      margin-top: 20px
    }
    &__input{
      margin-bottom: 15px;
    }
    &__input:last-child{
      margin-bottom: 30px;
      border: 3px solid;
    }
    &__link{
      text-decoration: none;
      color:#409EFF
    }
  }
</style>