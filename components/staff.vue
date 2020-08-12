<template>
  <div>
  <h1 class="title">Directors</h1>
    <section>
      <div v-for="Director in Directors" :key="Director.id">
        <div class="card">
          <div class="card-content">
            <div class="media">
              <div class="media-left">
                <figure class="image is-48x48">
                  <img v-bind:src="Director.logo" alt="Placeholder image" />
                </figure>
              </div>
              <div class="media-content">
                <p class="title is-4">{{ Director.name }}</p>
                <p class="subtitle is-6">{{ Director.role }}</p>
              </div>
            </div>
            <div class="content" id="desc">
              <p>{{ Director.desc }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
      <h1 class="title">Admins</h1>
    <section>
      <div v-for="Admin in Admins" :key="Admin.id">
        <div class="card">
          <div class="card-content">
            <div class="media">
              <div class="media-left">
                <figure class="image is-48x48">
                  <img v-bind:src="Admin.logo" alt="Placeholder image" />
                </figure>
              </div>
              <div class="media-content">
                <p class="title is-4">{{ Admin.name }}</p>
                <p class="subtitle is-6">{{ Admin.role }}</p>
              </div>
            </div>
            <div class="content" id="desc">
              <p>{{ Admin.desc }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <h1 class="title">Mods</h1>
    <section>
      <div v-for="Mod in Mods" :key="Mod.id">
        <div class="card">
          <div class="card-content">
            <div class="media">
              <div class="media-left">
                <figure class="image is-48x48">
                  <img v-bind:src="Mod.logo" alt="Placeholder image" />
                </figure>
              </div>
              <div class="media-content">
                <p class="title is-4">{{ Mod.name }}</p>
                <p class="subtitle is-6">{{ Mod.role }}</p>
              </div>
            </div>
            <div class="content" id="desc">
              <p>{{ Mod.desc }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <h1 class="title">Jr Mods</h1>
    <section>
      <div v-for="JrMod in JrMods" :key="JrMod.id">
        <div class="card">
          <div class="card-content">
            <div class="media">
              <div class="media-left">
                <figure class="image is-48x48">
                  <img v-bind:src="JrMod.logo" alt="Placeholder image" />
                </figure>
              </div>
              <div class="media-content">
                <p class="title is-4">{{ JrMod.name }}</p>
                <p class="subtitle is-6">{{ JrMod.role }}</p>
              </div>
            </div>
            <div class="content" id="desc">
              <p>{{ JrMod.desc }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      Directors: [
        {
          id: '1',
          name: 'FishSticz',
          role: 'Director',
          logo:
            'https://cdn.discordapp.com/avatars/212783568663871489/127407f3d719b02444e101c0de538e4e.webp?size=128',
          desc:
            'One of the Founders of International Lodge Discord. I do a lot of things, But I mostly stream whatever i fell like! I was told to write something interesting here.',
        },
        {
          id: '2',
          name: 'lol hooudini',
          role: 'Director',
          logo:
            'https://cdn.discordapp.com/avatars/413665927175864320/a_4b0fcf026cf8c191097bf9f7a267cd64.png?size=128',
          desc:
            'One of the Founders of International Lodge Discord. I stream a lot on twitch.I am a discord designer and promoter.What was i ment to write here?',
        },
      ],
      Admins: [
        {
          id: '1',
          name: 'Ethan',
          role: 'Admin',
          logo:
            'https://cdn.discordapp.com/avatars/382928087203184651/614af368d51feed67c7951bc1a031546.png?size=128',
          desc:
            'An admin for the International Lodge Discord. I am a fullstack web dev and often stream this on my twitch. Hit me up if you need anything.',
        },
        {
          id: '2',
          name: 'SerialChiller',
          role: 'Admin',
          logo:
            'https://cdn.discordapp.com/avatars/482248970178002946/a_244ff291a09cfae253c9e07953979fd5.webp?size=128',
          desc:
            'Have not Streamed yet. But starting on it.So you can call me a streamer. I am a 3D Modeller in games,So more into backend in games.',
        },
      ],
      Mods: [
        {
          id: '1',
          name: 'FishSticz',
          role: 'Director',
          logo:
            'https://cdn.discordapp.com/avatars/212783568663871489/127407f3d719b02444e101c0de538e4e.webp?size=128',
          desc:
            'One of the Founders of International Lodge Discord. I do a lot of things, But I mostly stream whatever i fell like! I was told to write something interesting here.',
        },
        {
          id: '2',
          name: 'lol hooudini',
          role: 'Director',
          logo:
            'https://cdn.discordapp.com/avatars/413665927175864320/a_4b0fcf026cf8c191097bf9f7a267cd64.png?size=128',
          desc:
            'One of the Founders of International Lodge Discord. I stream a lot on twitch. I am a discord designer and promoter.What was i ment to write here?',
        },
      ],
     JrMods: [
        {
          id: '1',
          name: 'OutFox',
          role: 'Mod',
          logo:
            'https://cdn.discordapp.com/avatars/393877783551410179/d9a47b7e55fa15de859f1e4c8a139792.png?size=128',
          desc:
            'Everyone hates me, but I still love you all. So you can call me a simp, but I still love you all.',
        },
        {
          id: '2',
          name: 'Thequake4fun',
          role: 'Mod',
          logo:
            'https://cdn.discordapp.com/avatars/239441810555011077/6866cdae81a7127218c29ae7d6081ab7.png?size=128',
          desc:
            'I Stream a lot on twitch. I like having fun. I dont take offensive.',
        },
      ],
    }
  },
}
</script>

<style scoped>
section {
  min-height: 40vh;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

img {
  border-radius: 50%;
}

.card {
  text-align: center;
  max-width: 320px;
  margin: 20px;
  height: 300px;
}

h1 {
    margin: 10px;
    text-align: center;
}
</style>
