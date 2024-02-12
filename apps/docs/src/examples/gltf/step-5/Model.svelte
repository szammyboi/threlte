<script lang="ts">
  import { T } from '@threlte/core'
  import { GLTF, useGltfAnimations } from '@threlte/extras'
  
  const { gltf, actions } = useGltfAnimations<'Take 001'>() 

  $: $actions['Take 001']?.play()
</script>

<GLTF
  bind:gltf={$gltf}
  url="/models/LittlestTokyo.glb"
  useDraco={true}
/>