<script>
  import { fadeIn, fadeOut } from "../utils/page_fade";
  import Article from "../components/Article.svelte";
  import Header from "../components/Header.svelte";
  import HeadlineTertiary from "../components/HeadlineTertiary.svelte";
  import SmallHero from "../components/SmallHero.svelte";
  import List from "../components/List.svelte";
  import ListItem from "../components/ListItem.svelte";
  import SimpleListItem from "../components/SimpleListItem.svelte";
  import OutgoingLink from "../components/OutgoingLink.svelte";
  import Spacing from "../components/Spacing.svelte";

  export let speakingUpcoming = [
    
  ];

  export let speakingPast = [
    {
      title: "Unleashing the Power of AI: Integrating Tiptap, OpenAI, and Vue.js",
      event: "Vuejs Amsterdam",
      eventSrc: "https://vuejs.amsterdam/program",
      location: "Amsterdam",
      date: "29/02/2024",
      emoji: "netherlands",
    },
    {
      title: "Unleashing the Power of AI: Integrating Tiptap, OpenAI, and Vue.js",
      event: "vueday 2023",
      eventSrc: "https://2023.vueday.it/index.html",
      location: "Verona",
      date: "10/11/2023",
      emoji: "italy",
    },
    {
      title: "Unleashing the Power of AI: Integrating Tiptap, OpenAI, and Vue.js",
      event: "MunichJS September Meetup",
      eventSrc: "https://www.meetup.com/munichjs-user-group/events/295733864/",
      location: "Alasco, Munich",
      date: "13/09/2023",
      emoji: "germany",
    },
    {
      title: "Create and Style a Project Creation Form",
      event: "Vue.js Forge",
      eventSrc: "https://vuejsforge.com/episode-4",
      videoSrc: "https://www.youtube.com/watch?v=7Sf9vp5hnJ0",
      location: "online",
      date: "02/08/2023",
      emoji: "www",
    },
    {
      title: "Session about Rich Text Editors",
      event: "Vue.js Conf",
      eventSrc: "https://jscraftcamp.org/",
      location: "Munich",
      date: "30/07/2023",
      emoji: "germany",
    },
    {
      title: "Generate Social Images with DALL-E",
      event: "Vue.js Forge",
      eventSrc: "https://vuejsforge.com/episode-3",
      videoSrc: "https://www.youtube.com/watch?v=seSh58Ya3IA",
      location: "online",
      date: "04/05/2023",
      emoji: "www",
    },
    {
      title: "State Management with Composition API",
      event: "Vue.js Toronto",
      eventSrc: "https://www.youtube.com/watch?v=MgtQ9t74mhw",
      location: "online",
      date: "22/11/2021",
      emoji: "www",
    },
    {
      title: "MC Vue.js Conf Berlin",
      event: "Vue.js Conf",
      location: "online",
      date: "05/10/2022",
      emoji: "germany",
    },
    {
      title: "State Management with Composition API",
      event: "Vue.js Roadshow",
      eventSrc: "https://barcelona.vuejs.amsterdam/",
      location: "Barcelona",
      date: "01/07/2022",
      emoji: "spain",
    },
    {
      title: "State Management with Composition API",
      event: "Vue.js Amsterdam",
      eventSrc: "https://www.vuejs.amsterdam/program",
      location: "Amsterdam",
      date: "03/06/2022",
      emoji: "netherlands",
    },
    {
      title: "Modern State Management with Vue 3",
      event: "GitNation",
      eventSrc: "https://portal.gitnation.org/contents/modern-state-management-with-vue-3",
      location: "online",
      date: "21/10/2021",
      emoji: "www",
    },
    {
      title: "Horizonterweiterung: State Management mit Composables",
      event: "enterJS VueDay",
      eventSrc: "https://enterjs.de/vueday.php",
      location: "online",
      date: "15/06/2021",
      emoji: "www",
    },
    {
      title: "Microfrontends: The Good, The Bad and The Ugly",
      event: "JSWorld Conference",
      eventSrc: "https://frontenddeveloperlove.com/",
      location: "online",
      slidesSrc:
        "https://de.slideshare.net/VanessaBhner/microfrontends-the-good-the-bad-and-the-ugly",
      date: "23/02/2021",
      emoji: "www",
    },
    {
      title: "Microfrontends: The Good, The Bad and The Ugly",
      event: "Munich Frontend Conference",
      eventSrc: "https://frontconf.com/",
      location: "Munich",
      slidesSrc: "https://slides.com/vannsl/microfrontends#/",
      date: "21/03/2020",
      emoji: "germany",
    },
    {
      title: "Microfrontends: The Good, The Bad and The Ugly",
      event: "Code is Colorful",
      eventSrc:
        "https://www.meetup.com/de-DE/SinnerSchrader-Frankfurt/events/268136278/",
      location: "Frankfurt",
      slidesSrc: "https://slides.com/vannsl/microfrontends#/",
      date: "25/02/2020",
      emoji: "germany",
    },
    {
      title: "Microfrontends: The Good, The Bad and The Ugly",
      event: "Code is Colorful",
      eventSrc: "https://www.meetup.com/de-DE/S2talks/events/267803544/",
      location: "Prague",
      slidesSrc: "https://slides.com/vannsl/microfrontends#/",
      date: "28/01/2020",
      emoji: "czech-republic",
    },
    {
      title: "Microfrontends: The Good, The Bad and The Ugly",
      event: "Code is Colorful",
      eventSrc:
        "https://www.meetup.com/de-DE/SinnerSchrader-Munich-Events/events/267755040/",
      location: "Munich",
      slidesSrc: "https://slides.com/vannsl/microfrontends#/",
      date: "22/01/2020",
      emoji: "germany",
    },
    {
      title: "Microfrontends: The Good, The Bad and The Ugly",
      event: "HHjs",
      eventSrc: "https://www.meetup.com/de-DE/hamburg-js/events/266723104/",
      location: "Hamburg",
      slidesSrc: "https://slides.com/vannsl/microfrontends#/",
      date: "11/12/2019",
      emoji: "germany",
    },
    {
      title: "Accidentally JAM Stack",
      event: "ScriptConf",
      eventSrc: "https://scriptconf.org/#jam",
      location: "Linz",
      videoSrc: "https://www.youtube.com/watch?v=G20P46_4L4A",
      date: "24/10/2019",
      emoji: "austria",
    },
    {
      title: "Why I decided to speak at Conferences",
      event: "Developer Relations",
      eventSrc: "https://www.meetup.com/de-DE/Dev-Rel-Munich/events/264890582/",
      location: "Munich",
      slidesSrc: "https://slides.com/vannsl/public-speaking#/",
      date: "20/09/2019",
      emoji: "germany",
    },
    {
      title: "Adventure Time: Let's build a website in 2019",
      event: "FrankenJS",
      eventSrc: "https://www.meetup.com/de-DE/FrankenJS/events/263000814/",
      location: "Nuremberg",
      slidesSrc: "https://slides.com/vannsl/adventure-time-franken-js#/",
      date: "29/07/2019",
      emoji: "germany",
    },
    {
      title: "Server-Side Rendering using Nuxt.js",
      event: "workerConf",
      eventSrc: "https://worker.sh/index#schedule",
      location: "Dornbirn",
      slidesSrc: "https://slides.com/vannsl/workerconf-nuxt#/",
      date: "28/06/2019",
      emoji: "austria",
    },
    {
      title: "Vue.js: Entstehung, Einsatzgebiete und Zukunftsprognosen",
      event: "enterJS",
      eventSrc:
        "https://enterjs.de/2019/single?id=8374&vue.js%3A-entstehung%2C-einsatzgebiete-und-zukunftsprognosen",
      location: "Darmstadt",
      date: "26/06/2019",
      emoji: "germany",
    },
    {
      title: "From Legacy to Vue.js",
      event: "iJS International JavaScript Conference",
      eventSrc:
        "https://javascript-conference.com/vue-js/from-legacy-to-vue-js/",
      location: "London",
      date: "14/05/2019",
      emoji: "united-kingdom",
    },
    {
      title: "Lightning: Nuxt.js <3 TailwindCSS",
      event: "FrontConf",
      eventSrc: "https://frontconf.com/",
      location: "Munich",
      date: "27/04/2019",
      emoji: "germany",
    },
    {
      title:
        "The VUE(.js)ture is here – endlich erweiter- und wartbare Webapplikationen?",
      event: "JavaScript Days",
      eventSrc:
        "https://javascript-days.de/javascript/the-vue-jsture-is-here-endlich-erweiter-und-wartbare-webapplikationen/",
      location: "Munich",
      date: "20/03/2019",
      emoji: "germany",
    },
    {
      title:
        "How to build a static website in two and a half days with Nuxt and TailwindCSS",
      event: "TechDivision Tech Talk",
      eventSrc: "https://www.techdivision.com/unternehmen/veranstaltungen.html",
      location: "Munich",
      date: "21/02/2019",
      emoji: "germany",
    },
    {
      title: "New website in two and a half days",
      event: "Code is Colorful",
      eventSrc:
        "https://www.meetup.com/de-DE/sinnerschrader-hamburg/events/256937241/",
      location: "Hamburg",
      date: "07/02/2019",
      emoji: "germany",
    },
    {
      title:
        "How to build a static website in two and a half days with Nuxt and TailwindCSS",
      event: "Frontend Developers",
      eventSrc:
        "https://www.meetup.com/de-DE/Munich-Frontend-Developers/events/256146257/",
      location: "Munich",
      date: "22/11/2018",
      codebases: [
        {
          src: "https://github.com/Vannsl/ausbaufaehig-podcast",
        },
      ],
      emoji: "germany",
    },
    {
      title: "Vue Single File Components and Composing",
      event: "TechDivision Tech Talk",
      eventSrc:
        "https://www.meetup.com/de-DE/TechDivision-TechTalk-Munchen/events/254404298/",
      location: "Munich",
      date: "20/09/2018",
      emoji: "germany",
    },
    {
      title: "Vue.js Component Tools",
      event: "Vue.js",
      eventSrc: "https://www.meetup.com/de-DE/Vue-js-Munich/events/253336909/",
      location: "Munich",
      date: "08/08/2018",
      slidesSrc: "https://de.slideshare.net/VanessaBhner/vuejs-component-tools",
      codebases: [
        {
          src: "https://github.com/Vannsl/Vue-Composing-Components",
        },
      ],
      emoji: "germany",
    },
    {
      title: "Pain Free Frontend Development",
      event: "PyConWeb",
      eventSrc: "https://2018.pyconweb.com/talks/30-06-2018/vuejs-talk",
      location: "Munich",
      date: "30/06/2018",
      slidesSrc: "https://de.slideshare.net/VanessaBhner/spa-flask-vue",
      codebases: [
        {
          src: "https://github.com/Vannsl/spa-flask-vue",
        },
      ],
      emoji: "germany",
    },
    {
      title: "State Transitions with Vue.js",
      event: "myposter Tech 'n' Drinks",
      eventSrc:
        "https://team.myposter.de/beer-bbq-vue-js-beim-tech-n-drinks-myposter/",
      location: "Munich",
      date: "12/06/2018 I",
      slidesSrc:
        "https://www.slideshare.net/myposter_techtalks/vue-state-transitions",
      codebases: [
        {
          src: "https://github.com/Vannsl/Vue-Transitions-Animations",
        },
        {
          src: "https://github.com/Vannsl/vue-router-transitions",
        },
      ],
      emoji: "germany",
    },
    {
      title: "Composing Components",
      event: "myposter Tech 'n' Drinks",
      eventSrc:
        "https://team.myposter.de/beer-bbq-vue-js-beim-tech-n-drinks-myposter/",
      location: "Munich",
      date: "12/06/2018 II",
      slidesSrc:
        "https://www.slideshare.net/myposter_techtalks/vue-composing-components",
      codebases: [
        {
          src: "https://github.com/Vannsl/Vue-Composing-Components",
        },
      ],
      emoji: "germany",
    },
  ];

  export let podcasts = [
    {
      title: "Svelte",
      src: "https://programmierbar.buzzsprout.com/176239/4238645-folge-64-svelte-mit-vanessa-bohner",
      publisher: "programmierbar",
      episode: "Folge 64",
      date: "19/06/2020",
      emoji: "podcast",
    },
    {
      title: "Svelte",
      src: "https://workingdraft.de/413/",
      publisher: "Working Draft",
      episode: "Revision 413",
      date: "18/02/2020",
      emoji: "podcast",
    },
    {
      title: "Micro Frontends mit Project Mosaic",
      src: "https://workingdraft.de/407/",
      publisher: "Working Draft",
      episode: "Revision 407",
      date: "07/01/2020",
      emoji: "podcast",
    },
    {
      title: "Frontend Testing",
      src: "https://workingdraft.de/375/",
      publisher: "Working Draft",
      episode: "Revision 375",
      date: "11/02/2019",
      emoji: "podcast",
    },
    {
      title: "Vue.js - Der Deep Dive",
      src: "https://workingdraft.de/367/",
      publisher: "Working Draft",
      episode: "Revision 367",
      date: "29/11/2018",
      emoji: "podcast",
    },
  ];

  export let interviews = [
    {
      title: "State of Vue March 2022",
      src: "https://www.youtube.com/watch?v=BUUupT4zfA0",
      publisher: "ThisDot",
      date: "24/03/2022",
      emoji: "videointerviews",
    },
    {
      title: "Panel discussion: State Management",
      src: "https://portal.gitnation.org/contents/panel-discussion",
      publisher: "GitNation",
      date: "21/10/2021",
      emoji: "videointerviews",
    },
    {
      title:
        "Vue.js: Nicht nur für neue Projekte eine gute Wahl | Vanessa Böhner im Interview | JS Days 2019",
      src: "https://www.youtube.com/watch?v=-tm2o4NHme4",
      publisher: "EntwickerAkadamie",
      date: "12/06/2019",
      emoji: "videointerviews",
    },
  ];

  export let mentoringUpcoming = [
  ];

  export let mentoringPast = [
  {
      title: "Create and Style a Project Creation Form",
      event: "Vue.js Forge 4",
      eventSrc: "https://www.youtube.com/watch?v=7Sf9vp5hnJ0",
      location: "Remote",
      date: "02/08/2023",
      emoji: "mentoring",
    },
  {
      title: "Generate Social Images with DALL-E",
      event: "Vue.js Forge 3",
      eventSrc: "https://www.youtube.com/watch?v=seSh58Ya3IA",
      location: "Remote",
      date: "03/05/2023",
      emoji: "mentoring",
    },
  {
      title: "State Management with Pinia",
      event: "Vue.js Conf",
      eventSrc: "https://conf.vuejs.de/workshops/state-management-with-pinia/",
      location: "Berlin",
      date: "04/10/2022",
      emoji: "mentoring",
    },
    {
      title: "Vue Vixens Full Day Workshop",
      event: "ScriptConf",
      eventSrc: "https://scriptconf.org/#workshops",
      location: "Linz",
      date: "24/10/2019",
      emoji: "mentoring",
    },
    {
      title: "Introduction to Nuxt.js",
      event: "workerConf",
      eventSrc: "https://scriptconf.org/#workshops",
      location: "Bregenz",
      date: "27/06/2019",
      slidesSrc: "https://slides.com/vannsl/nuxtjs-harry-potter#/",
      emoji: "mentoring",
    },
    {
      title: "JSDay - half a day full of JavaScript",
      event: "JSKongress Pre-Event @ SinnerSchrader",
      eventSrc:
        "https://www.meetup.com/de-DE/SinnerSchrader-Munich-Events/events/257780477/",
      location: "Munich",
      date: "10/03/2019",
      emoji: "mentoring",
    },
    {
      title: "ngGirls Full Day Workshop",
      location: "Munich",
      date: "24/11/2018",
      emoji: "mentoring",
    },
  ];
</script>

<svelte:head>
  <title>Vannsl | Speaking</title>
</svelte:head>

<main in:fadeIn out:fadeOut>
  <SmallHero segment="speaking" type="contain" />
  <Header title="talks" />
  <Spacing />
  <Article>
    <section class="flex items-center justify-center bg-gray-100 dark:bg-gray-900 py-12 px-4 mb-6">
      <div class="max-w-sm w-full bg-white dark:bg-gray-800 shadow-lg rounded-2xl p-6">
        <div class="text-center">
          <h2 class="text-2xl font-semibold text-gray-800 dark:text-gray-200">On Baby Break 👶</h2>
          <p class="text-gray-600 dark:text-gray-400 mt-4">
            I'm currently not attending any conferences as I'm on a baby break, focusing on my family during this special time.
          </p>
        </div>
      </div>
    </section>
    {#if speakingUpcoming.length > 0}
    <HeadlineTertiary>upcoming</HeadlineTertiary>
    <List>
      {#each speakingUpcoming as item (item.date)}
        <ListItem {item} />
      {/each}
    </List>
    {/if}
    <details open>
      <summary>
        <h3
          class=" text-tertiary dark:text-tertiary-light tracking-wider inline ml-4"
        >
          past
        </h3>
      </summary>
      <div class="mt-4">
        <List>
          {#each speakingPast as item (item.date)}
            <ListItem {item} />
          {/each}
        </List>
      </div>
    </details>
  </Article>
  <Spacing />
  <Header title="mentoring & workshops" />
  <Spacing />
  <Article>
    <List>
      {#each mentoringUpcoming as item (item.date)}
        <ListItem {item} />
      {/each}
    </List>
    <details open>
      <summary>
        <h3
          class=" text-tertiary dark:text-tertiary-light tracking-wider inline ml-4"
        >
          past
        </h3>
      </summary>
      <div class="mt-4">
        <List>
          {#each mentoringPast as item (item.date)}
            <ListItem {item} />
          {/each}
        </List>
      </div>
    </details>
  </Article>
  <Spacing />
  <Header title="podcasts & interviews" />
  <Spacing />
  <Article>
    <HeadlineTertiary>podcasts</HeadlineTertiary>
    <p class="mb-4 dark:text-gray-100">
      Since Nov' 2020 I'm a proud Co-host of the <OutgoingLink
        href="https://workingdraft.de/">Working Draft</OutgoingLink
      > podcast. I host the Frontend Testing Podcast <OutgoingLink
        href="https://www.workingdraft.de">expect(Exception)</OutgoingLink
      >. Below, find a list of podcasts where I've been a guest:
    </p>
    <List>
      {#each podcasts as item (item.date)}
        <SimpleListItem {item} />
      {/each}
    </List>
  </Article>
  <Article>
    <HeadlineTertiary>interviews</HeadlineTertiary>
    <List>
      {#each interviews as item (item.date)}
        <SimpleListItem {item} />
      {/each}
    </List>
  </Article>

  <Spacing />
  <Spacing />
</main>
