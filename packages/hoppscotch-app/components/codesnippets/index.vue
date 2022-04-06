<template>
  <div>
    <div class="sticky top-0 z-10 flex flex-col rounded-t bg-primary">
      <div class="flex justify-between flex-1 border-b border-dividerLight">
        <span
          v-tippy="{ theme: 'tooltip' }"
          :title="`${$t('code_snippet.select')}`"
          class="flex-1 bg-transparent border-b border-dividerLight select-wrapper"
        >
          <ButtonSecondary
            :label="`${$t('code_snippet.select')}`"
            class="flex-1 !justify-start pr-8 rounded-none"
          />
        </span>
        <div class="flex">
          <ButtonSecondary
            v-tippy="{ theme: 'tooltip' }"
            svg="settings"
            :title="$t('code_snippet.setting')"
          />
        </div>
      </div>
    </div>
  </div>
</template>
