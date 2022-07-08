<template>
  <main>
    <h1>{{ $t("back-soon") }}</h1>
    <div>
      <a href="https://discord.gg/invite/ENY2nV6" title="Discord">
        <img src="@/assets/svg/discord.svg" alt="Discord logo" />
      </a>
      <a href="https://www.twitch.tv/chartreusegaming" title="Twitch">
        <img src="@/assets/svg/twitch.svg" alt="Twitch logo" />
      </a>
      <a
        href="https://www.youtube.com/channel/UCJFJe1WVZtdQZuvkcS_2jSg"
        title="YouTube"
      >
        <img src="@/assets/svg/youtube.svg" alt="YouTube logo" />
      </a>
      <a href="https://twitter.com/chartreusegame" title="Twitter">
        <img src="@/assets/svg/twitter.svg" alt="Twitter logo" />
      </a>
      <a href="https://www.instagram.com/chartreusegaming/" title="Instagram">
        <img src="@/assets/svg/instagram.svg" alt="Instagram logo" />
      </a>
      <a href="https://www.facebook.com/chartreusegaming/" title="Facebook">
        <img src="@/assets/svg/facebook.svg" alt="Facebook logo" />
      </a>
      <a
        href="https://www.linkedin.com/company/chartreuse-gaming/"
        title="LinkedIn"
      >
        <img src="@/assets/svg/linkedin.svg" alt="LinkedIn logo" />
      </a>
      <a href="mailto:ChartreuseGGaming@gmail.com" title="Email">
        <img src="@/assets/svg/email.svg" alt="Email logo" />
      </a>
    </div>
  </main>
</template>

<script>
export default {
  name: "App",
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@800&display=swap");

* {
  margin: 0;
  padding: 0;
  font: inherit;
  font-weight: normal;
  color: white;
  box-sizing: border-box;
}

body {
  font-family: "Inter", "Helvetica", "Arial", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -o-user-select: none;
  user-select: none;
  overflow: hidden;
  background: rgb(15, 11, 61);
  background: -moz-linear-gradient(
    120deg,
    rgba(15, 11, 61, 1) 0%,
    rgba(23, 61, 9, 1) 100%
  );
  background: -webkit-linear-gradient(
    120deg,
    rgba(15, 11, 61, 1) 0%,
    rgba(23, 61, 9, 1) 100%
  );
  background: linear-gradient(
    120deg,
    rgba(15, 11, 61, 1) 0%,
    rgba(23, 61, 9, 1) 100%
  );
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#0f0b3d",endColorstr="#173d09",GradientType=1);
  color: white;

  main {
    padding: 20px;
    width: 100vw;
    height: 100vh;
    display: flex;
    flex-flow: column nowrap;
    align-items: center;
    justify-content: center;
    gap: 90px;
    background-image: url("@/assets/svg/bg-repeat.svg");
    background-size: cover;

    h1 {
      font-size: 3em;
      text-align: center;
      text-shadow: 0 10px 30px rgba(0, 0, 0, 0.8);
    }

    div {
      border: 5px solid white;
      border-radius: 16px;
      background-color: rgba(0, 0, 0, 0.3);
      padding: 8px 26px;
      display: flex;
      flex-flow: row wrap;
      align-items: center;
      justify-content: center;
      gap: 30px;
      box-shadow: 0 11px 15px -7px rgb(0 0 0 / 20%),
        0 24px 38px 3px rgb(0 0 0 / 14%), 0 9px 46px 8px rgb(0 0 0 / 12%);

      a {
        padding: 14px;
        transform: scale(1);
        transition: all 0.2s;
        text-align: center;

        &:hover {
          transform: scale(1.1);
        }

        & > * {
          width: 36px;
          height: 36px;
        }

        @media only screen and (max-width: 850px) {
          flex: 0 0 16%;
        }
      }
    }
  }
}
</style>
