<script setup>
import ImageHeadComponent from "@/components/image/imageHead.vue"
import ImageTextComponent from "@/components/image/imageText.vue"
import ButtonComponent from "@/components/button.vue"
import LabelComponent from "@/components/label.vue"

const parentHandler = () => console.log (Çalışıyor)
</script>

<template>
  <div class="wrapped">

    <section>
      <img src="src/Images/img/Card.jpg" alt="">
      <ImageHeadComponent head='Update payment method'></ImageHeadComponent>
      <ImageTextComponent text='Update your card details.'></ImageTextComponent>
    </section>

    <div class="inputPart">

      <section>
        <LabelComponent text='Name on card'></LabelComponent>
        <input type="text" class="tall">
      </section>

      <section>
        <LabelComponent text='Expiry'></LabelComponent>
        <input type="month" class="short">
      </section>

    </div>

    <div class="inputPart">

      <section>
        <LabelComponent text='Card number'></LabelComponent>
        <input type="number" class="tall">
      </section>

      <section>
        <LabelComponent text='CVV' size='short'></LabelComponent>
        <input type="password" class="short">
      </section>

    </div>


    <div class="buttonPart">
      <ButtonComponent button="Cancel"></ButtonComponent>
      <ButtonComponent button="Update" ></ButtonComponent>
    </div>

  </div>

  <div class="wrapped">

    <section>
      <video src="src/components/video/video.mp4" controls='controls' ></video>
      <ImageHeadComponent head='You video has been uploaded!'></ImageHeadComponent>
      <ImageTextComponent text='You are video has finished uploading and is live.'></ImageTextComponent>
    </section>


    <div class="inputPart">

      <section>
        <LabelComponent text='Share link'></LabelComponent>
        <input type="text" class="tall" value="https://www.youtube.com/watch?v=vmHoGicPQQQ">
      </section>

      <section>
        <LabelComponent text=''></LabelComponent>
        <input type="text" value="Copy" class="short">
      </section>

    </div>


    <div class="buttonPart">
      <ButtonComponent button="Skip" @handler="parentHandler"></ButtonComponent>
      <ButtonComponent button="Next"  ></ButtonComponent>
    </div>

  </div>
</template>

<style scoped>
img {
  
  height: 325px;
  border-radius: 10px;
  box-shadow: 0 0px 1px 0px gray;
}

video {
 overflow: auto;
  
  border-radius: 10px;
  box-shadow: 0 0px 1px 0px gray;
}

.wrapped {
  padding: 25px;
  width: 550px;
  height: 100%;
  background-color: white;
  border-radius: 10px;
  margin: 25px;
}

section {
  display: flex;
  flex-direction: column;
}

.inputPart {
  margin: 10px 0px;
  display: flex;
  flex-direction: row;
  gap: 5px;
  
  justify-content: space-between;
  align-items: flex-end;
}

.buttonPart {
  display: flex;
  flex-direction: row;
  gap: 10px;
  justify-content: space-between;
  margin-top: 15px;
}

.tall {
  padding: 8px 50px;
  border-radius: 5px;
  background-color: white;
  border: 1px solid black;
}

.short {
  padding: 8px 10px;
  border-radius: 5px;
  background-color: white;
  border: 1px solid black;
}
</style>
