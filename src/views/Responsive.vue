<template>

  <title-bar :title-stack="titleStack" />

  <hero-bar>Responsive layout</hero-bar>

  <titled-section>
    Mobile & Tablet
  </titled-section>

  <main-section>
    <div class="md:w-10/12 shadow-2xl md:mx-auto rounded-3xl border-8 border-white">
      <img
        src="https://justboil.me/images/one-tailwind/repository-preview-m-hi-res.png"
        class="block rounded-3xl"
      >
    </div>
  </main-section>

  <titled-section>
    Small laptop 1024px
  </titled-section>

  <main-section>
    <div class="md:w-10/12 shadow-2xl md:mx-auto rounded-3xl border-8 border-white">
      <img
        src="https://justboil.me/images/one-tailwind/repository-preview-1024.png"
        class="block rounded-3xl"
      >
    </div>
  </main-section>

  <main-section>
    <div class="md:w-10/12 shadow-2xl md:mx-auto rounded-3xl border-8 border-white">
      <img
        src="https://justboil.me/images/one-tailwind/repository-preview-1024-menu.png"
        class="block rounded-3xl"
      >
    </div>
  </main-section>

  <titled-section>
    Laptop & desktop
  </titled-section>

  <main-section>
    <div class="md:w-10/12 shadow-2xl md:mx-auto rounded-3xl border-8 border-white">
      <img
        src="https://justboil.me/images/one-tailwind/repository-preview-no-libs.png"
        class="block rounded-3xl"
      >
    </div>
  </main-section>

  <bottom-other-pages-section />
</template>

<script>
import { ref } from 'vue'
import TitleBar from '@/components/TitleBar'
import HeroBar from '@/components/HeroBar'
import TitledSection from '@/components/TitledSection'
import MainSection from '@/components/MainSection'
import BottomOtherPagesSection from '@/components/BottomOtherPagesSection'

export default {
  name: 'Responsive',
  components: {
    BottomOtherPagesSection,
    MainSection,
    TitledSection,
    HeroBar,
    TitleBar
  },
  setup () {
    const titleStack = ref(['Admin', 'Responsive layout'])

    return {
      titleStack
    }
  }
}
</script>
