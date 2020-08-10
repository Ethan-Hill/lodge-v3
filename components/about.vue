<template>
  <section>
    <div id="tiles" class="tile is-ancestor">
      <div class="tile is-vertical is-12">
        <div class="tile">
          <div class="tile is-parent is-vertical">
            <article class="tile is-child notification is-primary">
              <p class="title">Who are we?</p>
              <br />
              <p class="subtitle">
                We are a small discord community, That focuses on the "small"
                streamers. We Strive for positivity and equality. Join us today,
                let's make the interwebs less toxic.
              </p>
            </article>
            <article class="tile is-child notification is-warning">
              <p class="title">What to expect</p>
              <ul>
                <li>
                  <p>•Surrounded By People Who Share Similar Values</p>
                </li>
                <li><p>•So Much To Learn, So Much To Teach</p></li>
                <li><p>•Connect To People On A Deep Level</p></li>
                <li><p>•Push Each Other For The Better</p></li>
                <li>
                  <p>
                    •Find Teammates Easily For Projects You Want To Start
                  </p>
                </li>
                <li><p>•Always Something Fun Going On</p></li>
                <li><p>•Expenses Will Lower</p></li>
                <li><p>•Make Friends For Life</p></li>
              </ul>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child notification is-info">
              <p class="title">Our server</p>
              <div style="padding-top: 18px;"></div>
              <iframe
                style="height: 400px;"
                class="discord"
                src="https://discordapp.com/widget?id=702951112390606889&theme=dark"
                width="500"
              ></iframe>
              <br>
              <a href="https://discord.gg/nVHHYQu"><b-button rounded type="is-success">Connect</b-button></a>
              <div style="padding-bottom: 18px;"></div>
            </article>
          </div>
        </div>
        <div class="tile is-parent">
          <article class="tile is-child notification is-danger">
            <p class="title">Socials</p>
            <p class="subtitle">
              <a href="https://twitter.com/Int_Lodge"
                ><i class="fab fa-twitter-square" style="font-size: 45px;"></i
              ></a>
            </p>
            <div class="content">
              <!-- Content -->
            </div>
          </article>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import '@fortawesome/fontawesome-free'

export default {
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href:
            'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.14.0/css/all.min.css',
        },
      ],
    }
  },
}
</script>

<style scoped>
#tiles {
  margin: 0px 200px 0px 200px;
}

@media only screen and (max-width: 1000px) {
  #tiles {
    margin-top: 90% !important;
    margin: 40px;
  }
}

p {
  font-weight: bold;
}

section {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 88.5vh;
  width: 100vw;
}

.notification {
  text-align: center;
}
</style>
