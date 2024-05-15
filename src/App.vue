<script setup>
import HelloWorld from './components/HelloWorld.vue';
import axios from 'axios';
import {WDOTInitialization} from 'dop-website-sdk/src'; 
</script>
<script>
WDOTInitialization.setConfig({
    serviceNumber:10249,
    dotAccessToken:"7oGUQDmojFDLNqP+lj77clTq7SVpQ9/b/SgBCEyB9kL4kJcvn+XF++v4/oNUSZ0WI2nVYKDDckUSrcVnrkSWILdvUdow0PlKah3CJVVpj5wQEyafUSAxIjtZL292U4cs",
    combackUserLimitDays:14,
    dotEndPoint:"https://trk.analytics.wisetracker.co.kr/web/v1/dataRcv.do",
    adClkEndPoint:"https://trk.analytics.wisetracker.co.kr/ldsys/v1/clickDataRcv.do",
    adLandingEndPoint:"https://app.wisetracker.co.kr",
    includeUrl:"wisetracker.co.kr|research-draft.*.framer.app|localhost|192.168.1.61",
    excludeUrl:"",
    referrerExpire:7,
    firstEventSendMode : false
  })
  WDOTInitialization.init(); 
</script>
<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
