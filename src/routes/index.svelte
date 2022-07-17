<script lang="ts">
  import { store } from "../hooks/auth";
</script>

{#if $store != null}
  <div class="bg-slate-100 rounded-xl p-8 dark:bg-slate-800">
    <img
      class="w-24 h-24 rounded-full mx-auto"
      src="https://via.placeholder.com/150"
      alt=""
      width="384"
      height="512"
    />
    <div class="pt-6 text-center space-y-4">
      <AfterLogin />
    </div>
  </div>
{:else}
  <LoginComponents />
{/if}
