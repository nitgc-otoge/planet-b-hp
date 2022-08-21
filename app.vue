<script setup lang="ts">
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
  <NuxtLayout name="root">
    <NuxtLayout name="nav">
      <template #logo>
        <!-- TODO: ロゴの用意 -->
        <!-- <img src="@/assets/images/logo.jpg" class="w-48"/> -->
        PLANET-B
      </template>
      <template #nav-bar>
        <NavBar></NavBar>
      </template>
    </NuxtLayout>
    <NuxtPage></NuxtPage>
  </NuxtLayout>
</template>
