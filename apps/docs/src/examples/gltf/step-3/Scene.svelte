<script lang="ts">
  import { T } from '@threlte/core'
  import { OrbitControls } from '@threlte/extras'
  import Model from './Model.svelte'

</script>

<T.PerspectiveCamera
  makeDefault
  position={[5, 2, 5]}
  fov={25}
>
  <OrbitControls
    autoRotate
    enableDamping
  />
</T.PerspectiveCamera>

<T.AmbientLight />
<T.DirectionalLight position={[5, 10, 5]} />

<Model />
