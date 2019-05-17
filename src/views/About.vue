<template>
  <div>
    <v-img :src="require('@/assets/about-map.png')" />
    <v-parallax height="650" :src="require('@/assets/about-phoenix.png')">
      <v-container fluid>
        <v-flex md5 xs12 class="mt-5">
          <CardContent title="Phoenix, AZ" subtitle="33.4484° N, 112.0740° W">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer quis posuere ligula. Cras ullamcorper mi ex, non dictum urna pulvinar eu. Aliquam venenatis pellentesque quam. Pellentesque vestibulum bibendum diam, quis tristique sem eleifend vel. Ut in justo ornare, eleifend purus in, eleifend nisl. Nulla quam libero, molestie vel est ut, bibendum posuere ante. Phasellus non consequat purus. Nullam mattis scelerisque augue, eu tempor libero ultricies ac. Cras non leo diam.
            </p>
            <p>
              Nam tempus ullamcorper risus id posuere. Curabitur congue diam erat. Aliquam erat volutpat. Ut egestas ac tortor non euismod. Fusce porta nunc non semper convallis. Suspendisse auctor mattis lorem, fringilla feugiat arcu mollis nec. Ut eget porta tortor. Mauris volutpat lobortis odio ut efficitur. Etiam finibus nibh eu elit aliquam, ac blandit risus euismod. Aenean rutrum feugiat tellus ac varius. Donec sed libero ligula. Donec ut lobortis eros. Vestibulum dapibus dui massa, sed rhoncus quam sagittis ultrices.
            </p>
          </CardContent>
        </v-flex>
      </v-container>
    </v-parallax>
    <v-parallax height="650" :src="require('@/assets/about-west-palm-beach.png')">
      <v-container fluid>
        <v-flex md5 xs12 offset-md7 class="mt-5">
          <CardContent title="West Palm Beach, FL" subtitle="26.7153° N, 80.0534° W">
            <p>
              Ut pretium, ipsum vitae faucibus rutrum, ipsum enim aliquam nunc, a tristique erat tellus vel quam. Nunc sem justo, mollis eget tempus nec, facilisis quis nisl. Duis quis libero at enim venenatis rutrum nec eget dolor. Sed tincidunt magna quis nibh consequat, ac viverra diam sollicitudin. Quisque porta vehicula erat, maximus auctor magna blandit in. Nam vel enim quis dui tempus euismod vitae tempor diam. Maecenas quis vehicula nibh. Suspendisse eu mollis dui, in pretium augue. Morbi vitae rhoncus orci. In rhoncus feugiat porta. Cras posuere felis at nunc molestie malesuada.
            </p>
            <p>
              Vestibulum lacinia mollis lacus id tincidunt. Etiam at metus eu elit cursus euismod vitae ac dui. Mauris quis sollicitudin orci, sit amet iaculis felis. Nulla congue rhoncus dui a rutrum. Nulla id libero nulla. Proin massa dui, semper at mollis rutrum, egestas in purus. Pellentesque volutpat, mi vitae aliquet tincidunt, augue tellus accumsan quam, efficitur volutpat enim magna sit amet libero. Quisque sit amet ipsum sed orci finibus faucibus. Suspendisse non nunc varius, pharetra justo eget, varius sem.
            </p>
          </CardContent>
        </v-flex>
      </v-container>
    </v-parallax>
  </div>
</template>

<script>
  import CardContent from '@/components/CardContent'

  export default {
    components: {
      CardContent
    }
  }
</script>
