<template>

  
  <Page>
    <ActionBar title="Action Items">
        <ActionItem tap="onShare"
            ios.systemIcon="9" ios.position="left"
            android.systemIcon="ic_menu_share" android.position="actionBar"></ActionItem>
        <ActionItem tap="onDelete" text="delete" 
            ios.systemIcon="16" ios.position="right"
            android.position="popup"></ActionItem>
    </ActionBar>
    
    
    
    
    
    

    <AbsoluteLayout>
      <Label text="10,10" left="10" top="10" width="100" height="100" backgroundColor="#43b883">
        
      </Label>
      <HtmlView top="400" html="
    <div>
      <h1>HtmlView</h1>
    </div>
    <div class='box'>
      This is a box
    </div>
    "></HtmlView>
      <Button top="200"  left="300" class="my-button" text="Tap me!"></Button>
      <Label text="120,10" left="120" top="10" width="100" height="100" backgroundColor="#43b883"/>
      <Label text="10,120" left="10" top="120" width="100" height="100" backgroundColor="#43b883"/>
      <Label text="120,120" left="120" top="120" width="100" height="100" backgroundColor="#43b883"/>
    </AbsoluteLayout>
  </Page>
</template>

<script lang="ts">
// import { HtmlView } from "@nativescript/core";
  import Vue from "nativescript-vue";

  export default Vue.extend({
    computed: {
      message() {
        return "Blank {N}-Vue app";
      }
    },
  });
</script>

<style scoped lang="scss">
  @import '@nativescript/theme/scss/variables/blue';

  // Custom styles
  .fas {
    @include colorize($color: accent);
  }

  .info {
    font-size: 50;
    horizontal-align: center;
    vertical-align: center;
  }
    .my-button {
    background-color: lightseagreen;
    border-color: black;
    border-radius: 20;
    border-width: 2;
    color: whitesmoke;
    font-size: 18;
    font-weight: bold;
    height: 100px;
    width: 200px;
}
</style>
