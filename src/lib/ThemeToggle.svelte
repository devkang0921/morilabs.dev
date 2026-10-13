<script lang="ts">
  import { onMount } from 'svelte';

  let dark = $state(true);

  function applyTheme(value: boolean) {
    dark = value;
    document.documentElement.dataset.theme = value ? 'dark' : 'light';
    const meta = document.querySelector('meta[name="theme-color"]');
    meta?.setAttribute('content', value ? '#131a29' : '#f6f7fb');
  }

  onMount(() => {
    let saved: string | null = null;
    try {
      saved = localStorage.getItem('morilabs-theme');
    } catch {
      // The toggle still works when browser storage is unavailable.
    }
    applyTheme(saved !== 'light');
  });

  function toggleTheme() {
    applyTheme(!dark);
    try {
      localStorage.setItem('morilabs-theme', dark ? 'dark' : 'light');
    } catch {
      // Keep the current choice for this visit when storage is unavailable.
    }
  }
</script>

<button
  class="theme-toggle"
  type="button"
  onclick={toggleTheme}
  aria-label="다크 모드"
  aria-pressed={dark}
  title={dark ? '라이트 모드로 전환' : '다크 모드로 전환'}
>
  <span aria-hidden="true">{dark ? '☀' : '☾'}</span>
</button>
