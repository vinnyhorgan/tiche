<script>
  import { page } from "$app/stores";

  import IconHome from "~icons/mdi/home";
  import IconUser from "~icons/mdi/user";
  import IconGear from "~icons/mdi/gear";
  import IconBell from "~icons/mdi/bell";
</script>

<div class="min-h-screen flex flex-col">
  <div class="navbar bg-base-100">
    <div class="flex-1">
      <a href="/" class="btn btn-ghost text-xl">Tiche</a>
    </div>
    <div class="flex-none">
      <button class="btn btn-circle btn-ghost">
        <div class="indicator">
          <IconBell />
          <span class="badge badge-xs badge-primary indicator-item"></span>
        </div>
      </button>
    </div>
  </div>

  <div class="bg-base-200 flex-1 flex items-center justify-center">
    <slot />
  </div>
</div>

<div class="btm-nav">
  <a
    href="/main"
    class={$page.route.id === "/main" ? "active text-primary" : ""}
  >
    <IconHome />
  </a>
  <a
    href="/main/profile"
    class={$page.route.id === "/main/profile" ? "active text-primary" : ""}
  >
    <IconUser />
  </a>
  <a
    href="/main/settings"
    class={$page.route.id === "/main/settings" ? "active text-primary" : ""}
  >
    <IconGear />
  </a>
</div>
