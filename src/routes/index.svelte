<script>
  import { Card, Button, Label, Input } from "flowbite-svelte";

  let id = "";

  function login() {
    if (id != "") {
      console.log("login ... ", id);
    }
  }
</script>

<div class="box">
  <Card class="w-full max-w-md">
    <form class="flex flex-col space-y-6">
      <h3
        class="text-xl font-medium text-gray-900 dark:text-white"
        style="text-align: center;"
      >
        WIND - 斗地主
      </h3>

      <Label class="space-y-2">
        <span>你的ID：</span>
        <Input name="email" placeholder="张三" required bind:value={id} />
      </Label>

      <Button class="w-full" on:click={login}>登陆</Button>
    </form>
  </Card>
</div>

<style>
  .box {
    display: flex;
    justify-content: center;
    align-items: center;

    margin-top: 50px;
  }
</style>
