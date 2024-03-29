<p align="center">
  <a href="https://vuetube.app/">
    <img src="https://cdn.discordapp.com/attachments/751596360108605500/983689395834089512/Part_of_VueTube.svg" alt="VueTube icon" width="500"/>
  </a>
  </br>
  <sub>Logo by <a href="https://github.com/afnzmn">@afnzmn</a></sub>
  </br>
  </br>
<strong>This example plugin will help you to develop your own plugins for VueTube.</strong>
</br>
The main VueTube repository can be found <a href="https://github.com/VueTube/VueTubeApp"> here.</a>
The documentation of plugins can be found <a href="https://vuetube.app/plugins/"> here.</a>
</p>

## Example plugin

```
module.exports = {
  manifest: {
    name: "Test plugin", // Required
    vuetube: "*",
    version: "1.0", // Required
    author: "Frontesque", // Required
    description: "A plugin to test how vuetube handles plugins // Add 'Hello, World!' to the home page.", // Required
    homepage: "https://github.com/Frontesque/VueTube-Example-Plugin",
    license: "GPL-3.0" // Required
  },

  /************************* 
   * Execute code on ALL VueTube pages
   ************************/
  global: function() {

  },

  /************************* 
   * Execute code on SPECIFIC VueTube pages
   * 
   * You can view what page you intend to inject code into by looking at `~/NUXT/pages/` in the main VueTube repo
   ************************/
  pages: {
    home: function() { // Execute code on JUST the home page

    }
  }

}
```

## Another repositories

<a href="https://github.com/VueTube/VueTubeApp"> VueTube App </a> <br>
<a href="https://github.com/VueTube/VueTube-Extractor"> VueTube Extractor </a> <br>
<a href="https://github.com/VueTube/vuetube-http"> VueTube HTTP </a>
