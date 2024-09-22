<script>
  import { onMount } from "svelte";
  import { themeChange } from "theme-change";

  onMount(() => {
    themeChange(false);
  });
</script>

<h1 class="text-3xl font-bold underline">Welcome to Tiche!</h1>

<a href="/login" class="link">To login page</a>
<a href="/register" class="link">To register page</a>
<a href="/main" class="link">To main page</a>

<select data-choose-theme>
  <option value="">Default</option>
  <option value="light">Light</option>
  <option value="cupcake">Cupcake</option>
  <option value="bumblebee">Bumblebee</option>
  <option value="emerald">Emerald</option>
  <option value="corporate">Corporate</option>
  <option value="synthwave">Synthwave</option>
  <option value="retro">Retro</option>
  <option value="cyberpunk">Cyberpunk</option>
  <option value="valentine">Valentine</option>
  <option value="halloween">Halloween</option>
  <option value="garden">Garden</option>
  <option value="forest">Forest</option>
  <option value="aqua">Aqua</option>
  <option value="lofi">Lofi</option>
  <option value="pastel">Pastel</option>
  <option value="fantasy">Fantasy</option>
  <option value="wireframe">Wireframe</option>
  <option value="black">Black</option>
  <option value="luxury">Luxury</option>
  <option value="dracula">Dracula</option>
  <option value="cmyk">CMYK</option>
  <option value="autumn">Autumn</option>
  <option value="business">Business</option>
  <option value="acid">Acid</option>
  <option value="lemonade">Lemonade</option>
  <option value="night">Night</option>
  <option value="coffee">Coffee</option>
  <option value="winter">Winter</option>
  <option value="dim">Dim</option>
  <option value="nord">Nord</option>
  <option value="sunset">Sunset</option>
</select>
