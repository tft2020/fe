<template>
  <div id="app">
    <my-button />
  </div>
</template>

<script>
  import MyButton from "./components/MyButton";
export default {
  name: "App",
  components: {MyButton},
  mounted() {
    // 時間限制:30m
    // 題目: 實作n個按鈕, 按鈕上顯示的數值為下面n個setTimeout的參數值, 並且正序排列,
    // 若點擊按鈕, 會將按鈕上的數值+1, 並且維持按鈕數值間的正序排列

    // 例如:
    // 第一個setTimeout參數為一個一維陣列[1, 3]
    // 第二個setTimeout參數為一個一維陣列[2, 4]
    // 顯示的結果為四顆按鈕, 正序排列, 畫面上按鈕上對應的數字為1, 2, 3, 4
    // 此時若點擊數字為1的按鈕一下, 畫面上按鈕對應的數字應為2, 2, 3, 4
    //
    setTimeout(() => {}, 4000, [1, 3, 2]);
    setTimeout(() => {}, 1000, [4, 2]);
    setTimeout(() => {}, 5000, [5]);
  },
};
</script>

<style>
</style>

