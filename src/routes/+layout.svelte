<script>
  import Button from "$lib/components/ui/button/button.svelte";
  import "../app.pcss";
  import { Camera, Upload } from "lucide-svelte";
</script>

<!-- nav bar -->
<div class="border-b fixed top-0 w-full bg-white">
  <div class="container h-16 flex items-center">
    <a href="/">
      <Camera />
    </a>

    <div class="ml-auto">
      <Button class="space-x-1">
        <Upload class="h-[1rem]" />
        <span>Upload</span>
      </Button>
    </div>
  </div>
</div>

<div class="pt-16 container">
  <slot />
</div>
