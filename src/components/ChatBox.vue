<template>
    <div class="chatList">
        <div class="chatListChild" />
    <div class="chatEntry">
      <div class="contactDetails">
        <div class="profileInfo">
          <div class="frameParent">
            <div class="whyDoWeNeedAWalletParent">
              <img
                class="whyDoWeNeedAWallet"
                loading="lazy"
                alt=""
                src="/Friends/ellipse-11@2x.png"
              />
              <div class="frameWrapper">
                <div class="anilParent">
                  <h1 class="anil">Anil</h1>
                  <div class="onlineLast">
                    Online - Last seen, 2.02pm
                  </div>
                </div>
              </div>
            </div>
            <div class="moreOptions">
              <img
                class="bithreeDotsVerticalIcon"
                loading="lazy"
                alt=""
                src="/Friends/bithreedotsvertical.svg"
              />
            </div>
          </div>
        </div>
        <div class="separator" />
      </div>
    </div>

    <!--  chat section  -->
    <div class="messagePreview">
      <div class="messageContainerParent">
        <div class="messageContainer">
          <div class="rectangleParent">
            <div class="frameChild" />
            <div class="heyThere">Hey There!</div>
    
          </div>
        </div>


        <div class="messageContainer">
          <div class="rectangleParent">
            <div class="frameChild" />
            <div class="heyThere">How are you?</div>
    
          </div>
        </div>

      </div>
    </div>
 <!-- sent messages -->

 <div class="chatMessages">
      <div class="sentMessageContainerParent">
        <div class="sentMessageContainer">
          <div class="messageContent">
            <div class="messageBackground" />
            <h2 class="hello">Hello!</h2>
          </div>
          <div class="today833pmWrapper">
            <div class="today833pm">Today, 8.33pm</div>
          </div>
        </div>
        <div class="sentMessageContainer">
          <div class="messageContent">
            <div class="messageBackground" />
            <h2 class="hello">I am fine</h2>
          </div>
          <div class="today833pmWrapper">
            <div class="today833pm">Today, 8.33pm</div>
          </div>
        </div>
      
      </div>
    </div>

<!-- input contaienr -->

<div class="inputContainerParent">
      <div class="inputContainer">
        <div class="rectangleContainer">
          <div class="frameInner" />
          <div class="antDesignpaperClipOutlinedParent">
            <img
              class="antDesignpaperClipOutlinedIcon"
              loading="lazy"
              alt=""
              src="/Friends/antdesignpaperclipoutlined.svg"
            />
            <div class="typeYourMessageHereWrapper">
              <h3 class="typeYourMessage">Type your message here...</h3>
            </div>
          </div>
          <div class="fluentemojiLaugh16RegularParent">
            <img
              class="fluentemojiLaugh16RegularIcon"
              loading="lazy"
              alt=""
              src="/Friends/fluentemojilaugh16regular.svg"
            />
            <div class="fluentcamera24RegularWrapper">
              <img
                class="fluentcamera24RegularIcon"
                loading="lazy"
                alt=""
                src="/Friends/fluentcamera24regular.svg"
              />
            </div>
          </div>
        </div>
      </div>
      <div class="frameDiv">
        <div class="rectangleDiv" />
        <img class="bimicFillIcon" alt="" src="/Friends/bimicfill.svg" />
      </div>
    </div>
    </div>

</template>
<script>
import { defineComponent } from "vue";
 

   export default defineComponent({
     name: "ChatBox",
  
   });
</script>
<style>
/* main container */
.chatList{
    background-color: aquamarine;
    justify-content: flex-start;
    display: flex;
    flex-direction: column;
    border-radius: var(--br-6xl);
    box-shadow: 0px 4px 5px 2px rgba(121, 197, 239, 0.38);
    background-color: var(--color-white);
    box-sizing: border-box;
    /* height:auto; */
    padding: var(--padding-10xl) var(--padding-4xl) var(--padding-11xl)
      var(--padding-15xl);
    height: 635px;
}
/* profile and top  bar */
/* .chatListChild {
    width: 952px;
    height: 1010px;
    position: relative;
    border-radius: var(--br-6xl);
    background-color: var(--color-white);
    box-shadow: 0px 4px 5px 2px rgba(121, 197, 239, 0.38);
    display: none;
    max-width: 100%;
  } */
  .chatEntry {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px 0px var(--padding-7xs);
    box-sizing: border-box;
    max-width: 100%;
  }
  .contactDetails {
    flex: 1;
    display: flex;
    flex-direction: column;
    /* align-items: flex-start; */
    /* justify-content: flex-start; */
    gap: var(--gap-xl-5);
    max-width: 100%;
  }
  .profileInfo {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px 0px var(--padding-9xs);
    box-sizing: border-box;
    max-width: 100%;
  }
  .frameParent {
    flex: 1;
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    justify-content: space-between;
    max-width: 100%;
    gap: var(--gap-xl);
  }
  .whyDoWeNeedAWalletParent {
    width: 447px;
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    justify-content: flex-start;
    gap: var(--gap-6xl);
    max-width: 100%;
  }
  .bithreeDotsVerticalIcon {
    width: 40px;
    height: 40px;
    position: relative;
    z-index: 3;
  }
  .whyDoWeNeedAWallet {
    height: 59px;
    width: 59px;
    position: relative;
    border-radius: 50%;
    object-fit: cover;
    z-index: 3;
  }
  .anil {
    margin: 0;
    width: 90px;
    position: relative;
    font-size: var(--font-size-1xl);
    letter-spacing: 0.05em;
    font-weight: 600;
    font-family: var(--font-roboto);
    color: var(--color-darkslategray);
    text-align: left;
    display: inline-block;
    z-index: 3;
  }
  .onlineLast {
    align-self: stretch;
    position: relative;
    font-size: var(--font-size-lg);
    letter-spacing: 0.05em;
    font-weight: 300;
    font-family: var(--font-roboto);
    color: var(--color-darkslategray);
    text-align: left;
    z-index: 3;
  }
  .anilParent {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-12xs);
  }
  .frameWrapper {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-end;
    padding: 0px 0px var(--padding-9xs);
    box-sizing: border-box;
    min-width: 226px;
    max-width: 100%;
  }
  .moreOptions {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-end;
    padding: 0px 0px var(--padding-mid);
  }
  .separator {
    width: 876px;
    height: 1px;
    position: relative;
    border-top: 1px solid var(--color-darkgray);
    box-sizing: border-box;
    max-width: 100%;
    z-index: 3;
  }
  /* chat window */
  .messagePreview {
    width: 307px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-xl) var(--padding-10xl-5);
    box-sizing: border-box;
  }
  .messageContainerParent {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-4xl);
  }
  .messageContainer {
    width: 200px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 8px var(--padding-11xs);
    box-sizing: border-box;
  }
  .rectangleParent {
    flex: 1;
    border-radius: var(--br-6xl);
    background-color: var(--color-gainsboro);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-end;
    padding: var(--padding-sm) var(--padding-9xl);
    white-space: nowrap;
    z-index: 3;
  }
  .frameChild {
    height: 59px;
    width: 221px;
    position: relative;
    border-radius: var(--br-6xl);
    background-color: var(--color-gainsboro);
    display: none;
  }
  .heyThere {
    white-space: nowrap; /* Prevents text from wrapping */
    text-overflow: ellipsis;
    width: 152px;
    position: relative;
    font-size: var(--font-size-7xl);
    letter-spacing: 0.05em;
    font-family: var(--font-roboto);
    color: var(--color-darkslategray);
    text-align: left;
    display: inline-block;
    flex-shrink: 0;
    z-index: 4;
  }
  /* sent messages */

  .chatMessages {
    align-self: stretch;
    height: 233.5px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-end;
    padding: 0px var(--padding-8xl) var(--padding-base-5);
    box-sizing: border-box;
    max-width: 100%;
  }

  .sentMessageContainerParent {
    align-self: stretch;
    width: 437px;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: flex-start;
    gap: var(--gap-12xl);
    max-width: 100%;
  }

  .sentMessageContainer {
    width: 189px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .messageContent {
    width: 185px;
    height: 59px;
    position: relative;
  }

  .messageBackground {
    position: absolute;
    width: calc(100% - 4px);
    top: 0px;
    right: 4px;
    left: 0px;
    border-radius: var(--br-6xl);
    background-color: var(--color-blue);
    height: 59px;
    z-index: 3;
  }
  .hello {
    margin: 0;
    position: absolute;
    top: 15px;
    left: 53px;
    font-size: var(--font-size-7xl);
    letter-spacing: 0.05em;
    font-weight: 400;
    font-family: var(--font-roboto);
    color: var(--color-white);
    text-align: left;
    display: inline-block;
    width: 132px;
    height: 31px;
    z-index: 4;
  }
  .today833pmWrapper {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px 0px var(--padding-lg);
  }
  .today833pm {
    flex: 1;
    position: relative;
    font-size: var(--font-size-xl);
    letter-spacing: 0.05em;
    font-weight: 300;
    font-family: var(--font-roboto);
    color: var(--color-dimgray);
    text-align: left;
    z-index: 3;
  }
  .receivedBackgroundParent {
    align-self: stretch;
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .receivedBackground {
    align-self: stretch;
    flex: 1;
    position: relative;
    border-radius: var(--br-6xl);
    background-color: var(--color-blue);
    z-index: 3;
  }
  .today834pmWrapper {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-end;
  }
  .today834pm {
    width: 171px;
    position: relative;
    font-size: var(--font-size-xl);
    letter-spacing: 0.05em;
    font-weight: 300;
    font-family: var(--font-roboto);
    color: var(--color-dimgray);
    text-align: left;
    display: inline-block;
    flex-shrink: 0;
    z-index: 3;
  }
  /* input container */
  .inputContainerParent {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xl);
    max-width: 100%;
  }
  .inputContainer {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-11xs) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
  }
  .rectangleContainer {
    align-self: stretch;
    border-radius: var(--br-6xl);
    background-color: var(--color-aliceblue);
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    justify-content: space-between;
    padding: var(--padding-lgi) var(--padding-4xl) var(--padding-mid)
      var(--padding-3xl);
    box-sizing: border-box;
    max-width: 100%;
    gap: var(--gap-xl);
    z-index: 3;
  }
    .frameInner {
    height: 79px;
    width: 783px;
    position: relative;
    border-radius: var(--br-6xl);
    background-color: var(--color-aliceblue);
    display: none;
    max-width: 100%;
  }
  
  .antDesignpaperClipOutlinedParent {
    width: 420px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-12xl);
    max-width: 100%;
  }
  .antDesignpaperClipOutlinedIcon {
    height: 42px;
    width: 42px;
    position: relative;
    z-index: 4;
  }
  .typeYourMessageHereWrapper {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-6xs) 0px 0px;
    box-sizing: border-box;
    min-width: 226px;
    max-width: 100%;
  }
  .typeYourMessage {
    margin: 0;
    align-self: stretch;
    position: relative;
    font-size: var(--font-size-5xl);
    letter-spacing: 0.05em;
    line-height: 26px;
    font-weight: 300;
    font-family: var(--font-roboto);
    color: var(--color-darkslategray);
    text-align: left;
    z-index: 4;
  }
  .fluentemojiLaugh16RegularParent {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-6xl);
  }
  .fluentemojiLaugh16RegularIcon {
    height: 43px;
    width: 43px;
    position: relative;
    min-height: 43px;
    z-index: 4;
  }
  .fluentcamera24RegularWrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-11xs) 0px 0px;
  }
  .fluentcamera24RegularIcon {
    width: 38px;
    height: 38px;
    position: relative;
    z-index: 4;
  }
  .frameDiv {
    border-radius: var(--br-xl);
    background-color: var(--color-blue);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-xl) var(--padding-lg) var(--padding-xl)
      var(--padding-3xl);
    z-index: 3;
  }
  .rectangleDiv {
    height: 78px;
    width: 78px;
    position: relative;
    border-radius: var(--br-xl);
    background-color: var(--color-blue);
    display: none;
  }
</style>