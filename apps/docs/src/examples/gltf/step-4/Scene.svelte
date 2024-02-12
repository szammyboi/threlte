<script lang="ts">
  import { T } from '@threlte/core'
  import { OrbitControls } from '@threlte/extras'
  import Model from './Model.svelte'

</script>

<T.PerspectiveCamera
  makeDefault
  position={[600, 200, 600]}
  fov={45}
  near={10}
  far={10000}
>
  <OrbitControls
    autoRotate
    autoRotateSpeed={0.2}
    enableDamping
    enableZoom={false}
    target={[-60, -75, 0]}
  />
</T.PerspectiveCamera>
<T.AmbientLight />
<T.DirectionalLight position={[5, 10, 5]} />

<Model />
