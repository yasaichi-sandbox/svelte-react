<script lang="ts">
  import Button from './Button.svelte';
  import Heading from './Heading.svelte';

  const colors: string[] = ['#00ff00', '#ff0000', '#0000ff'];

  let count = 0;
  let color = colors[0];

  // TODO: Type this function.
  let handleClick = () => {
    count++;
    color = colors[Math.floor(Math.random() * 3)];
  };
</script>

<main>
  <Heading {count} />
  <Button {color} {handleClick} />
</main>
