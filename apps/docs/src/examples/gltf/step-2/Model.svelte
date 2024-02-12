<script lang="ts">
    import { T } from '@threlte/core'
    import { useGltf } from '@threlte/extras'

    const gltf = useGltf('/models/helmet/DamagedHelmet.gltf')
</script>

{#if $gltf}
  <T is={$gltf.nodes['node_damagedHelmet_-6514']} />
{/if}