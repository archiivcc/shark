<script lang="ts">
  import IconButton from "$lib/components/buttons/IconButton.svelte";
  import TextButton from "$lib/components/buttons/TextButton.svelte";
  import PageLayout from "$lib/components/layout/PageLayout.svelte";
  import Paragraph from "$lib/components/type/Paragraph.svelte";
</script>

<PageLayout>
  <h2 class="text-3xl font-semibold text-type-emphasized">About Us</h2>
  <Paragraph className="mt-2">
    SharkD is an advanced live markdown editor directly in your browser. It's built using SvelteKit
    and supports HTML as well as an extended markdown syntax all in the same file. SharkD is an open
    source project and an extremely opinionated one at that. All of the styles are made with custom
    tailwind css classes, and the markdown editor is built with Carta. This project is a fork of the original MarkD.
  </Paragraph>
  <div class="flex justify-center my-3">
    <TextButton
      onClick={() => open("https://github.com/itzcozi/markd", "_blank")}
      title="Original Source Code"
      className="w-full flex justify-center items-center">
    </TextButton>
    <TextButton
      onClick={() => open("https://github.com/archiivcc/sharkd", "_blank")}
      title="SharkD Source Code"
      className="w-full flex justify-center items-center">
    </TextButton>
  </div>
  <div class="flex flex-row gap-3 items-center my-2">
    <IconButton
      title="Email"
      onClick={() => window.open("mailto:chase@archiiv.cc")}
      className="w-full py-2 rounded-md">
      Email Us
    </IconButton>
  </div>
</PageLayout>
