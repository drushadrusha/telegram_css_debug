<template>
  <div class="container">
    <div class="card">
      <div class="card-body">
        --tg-theme-bg-color: <span :style="{ color: bg_color }"> {{ bg_color }} </span>;<br>
        --tg-theme-text-color: <span :style="{ color: text_color }"> {{ text_color }} </span>;<br>
        --tg-theme-hint-color: <span :style="{ color: hint_color }"> {{ hint_color }} </span>;<br>
        --tg-theme-link-color: <span :style="{ color: link_color }"> {{ link_color }} </span>;<br>
        --tg-theme-button-color: <span :style="{ color: button_color }"> {{ button_color }} </span>;<br>
        --tg-theme-button-text-color: <span :style="{ color: button_text_color }"> {{ button_text_color }} </span>;<br>
        --tg-theme-secondary-bg-color: <span :style="{ color: secondary_bg_color }"> {{ secondary_bg_color }} </span>;<br>
        --tg-theme-header-bg-color: <span :style="{ color: header_bg_color }"> {{ header_bg_color }} </span>;<br>
        --tg-theme-bottom-bar-bg-color: <span :style="{ color: bottom_bar_bg_color }"> {{ bottom_bar_bg_color }} </span>;<br>
        --tg-theme-accent-text-color: <span :style="{ color: accent_text_color }"> {{ accent_text_color }} </span>;<br>
        --tg-theme-section-bg-color: <span :style="{ color: section_bg_color }"> {{ section_bg_color }} </span>;<br>
        --tg-theme-section-header-text-color: <span :style="{ color: section_header_text_color }"> {{ section_header_text_color }} </span>;<br>
        --tg-theme-section-separator-color: <span :style="{ color: section_separator_color }"> {{ section_separator_color }} </span>;<br>
        --tg-theme-subtitle-text-color: <span :style="{ color: subtitle_text_color }"> {{ subtitle_text_color }} </span>;<br>
        --tg-theme-destructive-text-color: <span :style="{ color: destructive_text_color }"> {{ destructive_text_color }} </span>;<br>
      </div>
    </div>
  </div>

</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      bg_color: null,
      text_color: null,
      hint_color: null,
      link_color: null,
      button_color: null,
      button_text_color: null,
      secondary_bg_color: null,
      header_bg_color: null,
      bottom_bar_bg_color: null,
      accent_text_color: null,
      section_bg_color: null,
      section_header_text_color: null,
      section_separator_color: null,
      subtitle_text_color: null,
      destructive_text_color: null
    }
  },
  mounted() {
    if(window.Telegram && window.Telegram.WebApp){
      this.bg_color = window.Telegram.WebApp.themeParams.bg_color;
      this.text_color = window.Telegram.WebApp.themeParams.text_color;
      this.hint_color = window.Telegram.WebApp.themeParams.hint_color;
      this.link_color = window.Telegram.WebApp.themeParams.link_color;
      this.button_color = window.Telegram.WebApp.themeParams.button_color;
      this.button_text_color = window.Telegram.WebApp.themeParams.button_text_color;
      this.secondary_bg_color = window.Telegram.WebApp.themeParams.secondary_bg_color;
      this.header_bg_color = window.Telegram.WebApp.themeParams.header_bg_color;
      this.bottom_bar_bg_color = window.Telegram.WebApp.themeParams.bottom_bar_bg_color;
      this.accent_text_color = window.Telegram.WebApp.themeParams.accent_text_color;
      this.section_bg_color = window.Telegram.WebApp.themeParams.section_bg_color;
      this.section_header_text_color = window.Telegram.WebApp.themeParams.section_header_text_color;
      this.section_separator_color = window.Telegram.WebApp.themeParams.section_separator_color;
      this.subtitle_text_color = window.Telegram.WebApp.themeParams.subtitle_text_color;
      this.destructive_text_color = window.Telegram.WebApp.themeParams.destructive_text_color;
    }
  }
}
</script>

<style>
#app {
  margin-top: 60px;
}
</style>
