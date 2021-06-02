<template>
  <div class="box">
    <div id="chat">
      <BoxMessage />
    </div>
    <div id="input">
      <div class="value">
        <b-input class="input" type="text" />
      </div>
      <div class="icon">
        <b-button class="button">
          <IconSendMessage />
        </b-button>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.box {
  background: #fff;
  width: 500px;
  height: 500px;
  position: relative;
  border-radius: 10px;
  box-shadow: 0px 9px 9px rgba(50, 50, 50, 0.3);
  padding: 0.5rem;

  > #chat {
    height: 90%;
    width: 100%;
  }

  > #input {
    height: 10%;
    width: 100%;
    display: flex;
    justify-content: space-between;
    padding: 0 2rem;

    > .value {
      width: 83%;

      > .input {
        border: 1px solid #43b0f1;
        border-radius: 10px;
        height: 34px;
      }
    }

    > .icon {
      width: 10%;
      > .button {
        border-radius: 50%;
        border: 1px solid #43b0f1;
        width: 34px;
        height: 34px;
        padding: 0 3px 0 0;
        background: transparent;
      }
    }
  }
}
</style>
