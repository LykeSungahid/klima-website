<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
import { ref } from 'vue'

const show = ref(false)
const show1 = ref(false)
const show2 = ref(false)
const show3 = ref(false)
const show4 = ref(false)
const show5 = ref(false)
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading><h3><a @click="show = !show">Installations</a></h3></template>
     <Transition duration="550" name="nested">
    <div v-if="show" class="outer">
      <div class="inner">
        Lorem ipsum dolor sit amet. Ut recusandae assumenda eum voluptas veniam in sunt perferendis est voluptatem aperiam id cumque Quis. 
        Aut ipsum odit ut laboriosam voluptatem ut sequi perferendis ut architecto dolores eum odio corporis ad obcaecati voluptas eum ipsam repellat.
      </div>
    </div>
  </Transition>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
   <template #heading><h3><a @click="show1 = !show1">Project Design, Management and Estimates</a></h3></template>
     <Transition duration="550" name="nested">
    <div v-if="show1" class="outer">
      <div class="inner">
        Lorem ipsum dolor sit amet. Ut recusandae assumenda eum voluptas veniam in sunt perferendis est voluptatem aperiam id cumque Quis. 
        Aut ipsum odit ut laboriosam voluptatem ut sequi perferendis ut architecto dolores eum odio corporis ad obcaecati voluptas eum ipsam repellat.
      </div>
    </div>
  </Transition>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading><h3><a @click="show2 = !show2">Preventive Maintenance</a></h3></template>
     <Transition duration="550" name="nested">
      <div v-if="show2" class="outer">
        <div class="inner">
          Lorem ipsum dolor sit amet. Ut recusandae assumenda eum voluptas veniam in sunt perferendis est voluptatem aperiam id cumque Quis. 
          Aut ipsum odit ut laboriosam voluptatem ut sequi perferendis ut architecto dolores eum odio corporis ad obcaecati voluptas eum ipsam repellat.
        </div>
      </div>
    </Transition>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading><h3><a @click="show3 = !show3">Ventilation</a></h3></template>
      <Transition duration="550" name="nested">
        <div v-if="show3" class="outer">
          <div class="inner">
            Lorem ipsum dolor sit amet. Ut recusandae assumenda eum voluptas veniam in sunt perferendis est voluptatem aperiam id cumque Quis. 
            Aut ipsum odit ut laboriosam voluptatem ut sequi perferendis ut architecto dolores eum odio corporis ad obcaecati voluptas eum ipsam repellat.
          </div>
        </div>
      </Transition>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading><h3><a @click="show4 = !show4">Architectural and Civil Works</a></h3></template>
      <Transition duration="550" name="nested">
        <div v-if="show4" class="outer">
          <div class="inner">
            Lorem ipsum dolor sit amet. Ut recusandae assumenda eum voluptas veniam in sunt perferendis est voluptatem aperiam id cumque Quis. 
            Aut ipsum odit ut laboriosam voluptatem ut sequi perferendis ut architecto dolores eum odio corporis ad obcaecati voluptas eum ipsam repellat.
          </div>
        </div>
      </Transition>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading><h3><a @click="show5 = !show5">Other Mechanical - Related Works</a></h3></template>
      <Transition duration="550" name="nested">
        <div v-if="show5" class="outer">
          <div class="inner">
            Lorem ipsum dolor sit amet. Ut recusandae assumenda eum voluptas veniam in sunt perferendis est voluptatem aperiam id cumque Quis. 
            Aut ipsum odit ut laboriosam voluptatem ut sequi perferendis ut architecto dolores eum odio corporis ad obcaecati voluptas eum ipsam repellat.
          </div>
        </div>
      </Transition>
  </WelcomeItem>
</template>

<style>
.outer, .inner {
	background: #028799;
  padding: 30px;
  min-height: 100px;
}
  
.inner { 
  background: #b5fafa;
}
  
.nested-enter-active, .nested-leave-active {
	transition: all 0.3s ease-in-out;
}
/* delay leave of parent element */
.nested-leave-active {
  transition-delay: 0.25s;
}

.nested-enter-from,
.nested-leave-to {
  transform: translateY(30px);
  opacity: 0;
}

/* we can also transition nested elements using nested selectors */
.nested-enter-active .inner,
.nested-leave-active .inner { 
  transition: all 0.3s ease-in-out;
}
/* delay enter of nested element */
.nested-enter-active .inner {
	transition-delay: 0.25s;
}

.nested-enter-from .inner,
.nested-leave-to .inner {
  transform: translateX(30px);
  /*
  	Hack around a Chrome 96 bug in handling nested opacity transitions.
    This is not needed in other browsers or Chrome 99+ where the bug
    has been fixed.
  */
  opacity: 0.001;
}
a{
  color: rgb(17, 3, 223);
}
</style>