<template>
  <div id="app">
    <HelloWorld :msg="componentsArray[0].msg" :iframe="componentsArray[0].iframe"/>
    <HelloWorld :msg="componentsArray[1].msg" :iframe="componentsArray[1].iframe"/>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld
  },
  data() {
    return {
      componentsArray: [
        {
          msg: "React Components visualition in CodeSandbox!",
          iframe:
            '<iframe src="https://codesandbox.io/embed/basic-react-support-codesandbox-vqbc2?fontsize=14" title="basic-react-support-codesandbox" allow="geolocation; microphone; camera; midi; vr; accelerometer; gyroscope; payment; ambient-light-sensor; encrypted-media; usb" style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;" sandbox="allow-modals allow-forms allow-popups allow-scripts allow-same-origin"></iframe>'
        },
        {
          msg: "Vue Components visualition in CodeSandbox!",
          iframe:
            '<iframe src="https://codesandbox.io/embed/vue-template-irz1g?fontsize=14" title="Vue Template" allow="geolocation; microphone; camera; midi; vr; accelerometer; gyroscope; payment; ambient-light-sensor; encrypted-media; usb" style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;" sandbox="allow-modals allow-forms allow-popups allow-scripts allow-same-origin"></iframe>'
        }
      ]
    };
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
