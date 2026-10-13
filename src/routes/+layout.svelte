<script lang="ts">
  import '../app.css';
  import { onMount } from 'svelte';

  let { children } = $props();
  let progress = $state(0);

  onMount(() => {
    const updateProgress = () => {
      const distance = document.documentElement.scrollHeight - window.innerHeight;
      progress = distance > 0 ? Math.min(1, Math.max(0, window.scrollY / distance)) : 0;
    };
    const observer = new ResizeObserver(updateProgress);
    observer.observe(document.body);
    window.addEventListener('scroll', updateProgress, { passive: true });
    window.addEventListener('resize', updateProgress);
    updateProgress();
    return () => {
      observer.disconnect();
      window.removeEventListener('scroll', updateProgress);
      window.removeEventListener('resize', updateProgress);
    };
  });
</script>

<div class="scroll-progress" style:transform="scaleX({progress})" aria-hidden="true"></div>
{@render children()}
