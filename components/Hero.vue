<script >
data: () => {
    return {
      typeValue: "",
      typeStatus: false,
      displayTextArray: ["YouTuber", "Developer", "Blogger", "Designer", "Freelancer"],
      typingSpeed: 100,
      erasingSpeed: 100,
      newTextDelay: 2000,
      displayTextArrayIndex: 0,
      charIndex: 0,
    };
  }
</script>

<template>
  <section>
    <h1 class="text-5xl font-bold mt-20">Hello, I'm Waleed Alzubaidi!
        <span class="typed-text">{{ typeValue }}</span>
        <span class="blinking-cursor">|</span>
        <span class="cursor" :class="{ typing: typeStatus }">&nbsp;</span>
    </h1>

    <p class="text-base text-gray-900 p-2 italic">Spring Developer Advocate at VMware</p>
  </section>

  <section class="flex flex-col md:flex-row">
    <div class="md:w-3/4">
        <h2 class="text-3xl font bold mt-8">My Story</h2>
        <p class="text-lg py-2">
            I am Software Engineery living just outside of one of my favortite places in the world,
            Dobai, US. I am a self-taught programmer who firmly belives the you can accomplish 
            anything in this life if you put your mind to it,
            roll up your sleeves and are willing to put in the work.
        </p>
        <p class="text-lg py-2">
            I am Software Engineery living just outside of one of my favortite places in the world,
            Dobai, US. I am a self-taught programmer who firmly belives the you can accomplish 
            anything in this life if you put your mind to it,
            roll up your sleeves and are willing to put in the work.
        </p>
    </div>
    <img src="~/assets/images/user.png" class="w-1/2 md:max-w-sm p-8 mx-auto">
  </section>

  
</template>