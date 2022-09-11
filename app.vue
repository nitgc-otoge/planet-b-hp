<script setup lang="ts">
import PageHeader from './components/Common/PageHeader.vue'

const year = new Date().getFullYear()
</script>

<template>
  <Head>
    <Script>
      (function(d) { var config = { kitId: 'qzz6eet', scriptTimeout: 3000,
      async: true },
      h=d.documentElement,t=setTimeout(function(){h.className=h.className.replace(/\bwf-loading\b/g,"")+"
      wf-inactive";},config.scriptTimeout),tk=d.createElement("script"),f=false,s=d.getElementsByTagName("script")[0],a;h.className+="
      wf-loading";tk.src='https://use.typekit.net/'+config.kitId+'.js';tk.async=true;tk.onload=tk.onreadystatechange=function(){a=this.readyState;if(f||a&&a!="complete"&&a!="loaded")return;f=true;clearTimeout(t);try{Typekit.load(config)}catch(e){}};s.parentNode.insertBefore(tk,s)
      })(document);
    </Script>
  </Head>
  <div class="h-screen dark:bg-black dark:text-neutral-200">
    <NuxtLayout name="root">
      <NuxtLayout name="nav">
        <template #logo>
          <NuxtLink to="/">
            <img src="@/assets/images/logo.png" />
          </NuxtLink>
        </template>
        <template #nav-bar>
          <NavBar></NavBar>
        </template>
      </NuxtLayout>
      <PageHeader></PageHeader>
      <NuxtPage></NuxtPage>
      <div class="text-center">
        <span>© {{ year }} PLANET-B</span>
      </div>
    </NuxtLayout>
  </div>
</template>
