<template>
  <div class="playlist__item">
    <div class="playlist__track track">
      <div class="track__title">
        <div class="track__title-image">
          <svg class="track__title-svg">
            <use xlink:href="img/icon/sprite.svg#icon-note"></use>
          </svg>
        </div>
        <div class="track__title-text">
          <a class="track__title-link" href="http://">
            <slot name="title"></slot>
            <span class="track__title-span"><slot name="subtitle"></slot></span>
          </a>
        </div>
      </div>
      <div class="track__author">
        <a class="track__author-link" href="http://"
          ><slot name="author"></slot
        ></a>
      </div>
      <div class="track__album">
        <a class="track__album-link" href="http://"
          ><slot name="album"></slot
        ></a>
      </div>
      <div class="track__time">
        <svg class="track__time-svg">
          <use xlink:href="img/icon/sprite.svg#icon-like"></use>
        </svg>
        <span class="track__time-text"><slot name="duration"></slot></span>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
