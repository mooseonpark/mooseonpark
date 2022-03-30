### Hi there 👋

<!--
**mooseonpark/mooseonpark** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<div class="ocean">
  <div class="wave"></div>
  <div class="wave"></div>
</div>


body {
  height: 100vh;
  background-color: #000;
  overflow: hidden;
}

.wave,
.wave::before,
.wave::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  width: 250vw;
  height: 250vw;
  margin-left: -125vw;
  transform-origin: 50% 50%;
  background-color: transparent;
  border-radius: 38% 42%;
  box-shadow: inset 0 0 10vw rgba(255,0,255,0.8);
  animation: spin 16s infinite linear;
  mix-blend-mode: multiply;
}

.wave::before {
  width: 105%;
  height: 95%;
  margin-top: -125vw;
  transform-origin: 49% 51%;
  border-radius: 40% 38%;
  box-shadow: inset 0 0 10vw rgba(255,255,0,0.8);
  animation: spin 13s infinite linear;
}

.wave::after {
  width: 102%;
  height: 98%;
  margin-top: -125vw;
  transform-origin: 51% 49%;
  border-radius: 48% 42%;
  box-shadow: inset 0 0 10vw rgba(0,255,255,0.8);
  animation: spin 10s infinite linear;
}

@keyframes spin {
  100% { transform: rotate(360deg); }
}
