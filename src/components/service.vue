<template>
  <div class="box">
    <div class="img_bx" :style="setimage"></div>
    <div class="cont_box">
      <h6><span _msttexthash="148109" _msthash="36">NOTRE SERVICE</span></h6>
      <h1 _msttexthash="1574157" _msthash="37">
        Le confort est notre <br _istranslated="1" />
        priorité absolue pour vous
      </h1>
      <p _msttexthash="12594998" _msthash="38">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Explicabo minus ab porro
        id expedita facilis repudiandae dolorum maxime reprehenderit sit?
      </p>
      <ul>
        <li _msttexthash="662415" _msthash="39">Marquage national du parmium</li>
        <li _msttexthash="236171" _msthash="40">Viowing géré</li>
        <li _msttexthash="411476" _msthash="41">Frco, sans obligation</li>
        <li _msttexthash="376844" _msthash="42">Connaissance locale</li>
      </ul>
    </div>
  </div>
</template>
<script>
import { computed } from "vue";
export default {
  props: {
    image: String,
  },
  setup(props) {
    const setimage = computed(() => {
      return {
        backgroundImage: `url(${props.image})`,
      };
    });
    return {
      setimage,
    };
  },
};
</script>
