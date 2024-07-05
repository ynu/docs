---
layout: home
---

<script setup>
import { onMounted } from "vue";
import SwaggerUI from "swagger-ui";
import "swagger-ui/dist/swagger-ui.css";

onMounted(() => {
  SwaggerUI({
    dom_id: "#swagger",
    url: './rs-api.yaml'
  });
});
</script>

<div class="swagger" id="swagger"></div>

<style scoped>
/** add your custom style here **/
#swagger {
  border: 1px;
}
</style>