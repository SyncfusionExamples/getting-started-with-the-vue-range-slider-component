<script setup>
import { SliderComponent as EjsSlider } from "@syncfusion/ej2-vue-inputs";
const value = [30,70];
const type = 'Range';
const tooltip = { isVisible: true, showOn: 'Always', placement: 'After' };
const showButtons = true;
const ticks = { smallStep: 10, largeStep: 20, placement: 'After', showSmallTicks: true,
                format: '##.##km'};
const limits = { enabled: true, minStart: 10, minEnd: 30, maxStart: 40, maxEnd: 60 };
</script>

<template>
<ejs-slider :value="value" :type="type" :tooltip="tooltip" :showButtons="showButtons"
            :ticks="ticks" :limits="limits"></ejs-slider>
</template>

<style>
@import "../node_modules/@syncfusion/ej2-base/styles/material.css";
@import "../node_modules/@syncfusion/ej2-buttons/styles/material.css";
@import "../node_modules/@syncfusion/ej2-popups/styles/material.css";
@import "../node_modules/@syncfusion/ej2-vue-inputs/styles/material.css";
.e-control-wrapper.e-slider-container .e-slider .e-handle 
 {
  background-color: #f9920b;
  border-radius: 50%;
  border: 0;
} 
</style>
