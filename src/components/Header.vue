<template>
  <div class="row">
    <div class="col-sm-12">
      <h3>Quotes Added</h3>
      <div class="progress">
        <div
          :style="{width: (quotesCount/maxQuotes)*100 + '%'}"
          class="progress-bar"
          role="progressbar"
          aria-valuenow="60"
          aria-valuemin="0"
          aria-valuemax="100"
        >{{quotesCount}} / {{maxQuotes}}</div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["quotesCount", "maxQuotes"]
};
</script>

<style>
</style>