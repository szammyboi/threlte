<script lang="ts">
  import { T } from '@threlte/core'
  import { useGltf } from '@threlte/extras'
  import { MeshBasicMaterial } from 'three'

  const gltf = useGltf('/models/helmet/DamagedHelmet.gltf')
</script>

{#if $gltf}
  <T.Mesh
      geometry={$gltf.nodes['node_damagedHelmet_-6514'].geometry}
      material={new MeshBasicMaterial()}
  />
{/if}
