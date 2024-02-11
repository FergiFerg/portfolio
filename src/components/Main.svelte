<script>
  import Step from "./Step.svelte";

  /**
   * @type {any[]}
   */
  let steps = [
    // {
    //   name: " Store",
    //   icon: "fa-solid fa-cart-shopping",
    //   description:
    //     " Store is a a merchanising store created with Next.js, Commerce.js & Stripe! Commerce.js is a CMS for managing project and Stripe is used for all transaction handling.",
    // },
    // {
    //   name: "Utlimate Todos",
    //   icon: "fa-solid fa-list-check",
    //   description:
    //     "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
    // },
    // {
    //   name: "Pokdex",
    //   icon: "fa-solid fa-diagram-project",
    //   description:
    //     "Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).",
    // },
  ];

  let benefits = [
    {
      name: "Software Engineer - Incognito Software Systems",
      description: `
        <ul>
          <li>• Worked with clients to design solutions based on customer requirements.</li>
          <li>• Lead UI and QA effort by outlining test plan, delegating tasks to team members and publishing version releases.</li>
          <li>• Gathered requirements and developed test plans and test cases for new development projects.</li>
          <li>• Developed and implemented custom report creation programs in JavaScript and Python utilizing MongoDB to inject data into <a href="https://www.elastic.co/elastic-stack/?utm_campaign=Google-B-AMER-CA-Exact&utm_content=Brand-Core-ELK&utm_source=google&utm_medium=cpc&device=c&utm_term=elk%20elasticsearch&gad_source=1&gclid=CjwKCAiA_aGuBhACEiwAly57MdAv-dI_mT7XSaKe-ennTv2iqOFune4Qi8rZcGYvw_QcEuVJ8Ra2nRoCbpcQAvD_BwE" target="_blank" class="text-blue-500 underline">ELK</a> for customer visualizations.</li>
          <li>• Assisted customers with upgrades, troubleshooting services, and issue identification in production environments.</li>
          <li>• Application configuration and management in OpenShift, OpenStack, AWS, CloudStack.</li>
          <li>• Managed and Improved the CI/CD pipeline with Jenkins for the team.</li>
          <li>• Utilized open-source tools within development such as Kafka, Elasticsearch, and MongoDB in multi-cluster setups.</li>
        </ul>
      `,
    },
    {
      metric: "10x",
      name: "Computer Science Graduate",
      description: `I fell in love with the creativity and problem solving that is involved in developing and engineering innovative new online experiences. Starting off with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, Python, Java and backend programming, design, cloud services and much much more.`,
    },
    {
      name: "An excellent communicator",
      description: `Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.`,
    },
  ];
</script>

<main class="flex flex-col flex-1 p-4">
  <section
    id="introPage"
    class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
  >
    <div
      class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
    >
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi! I'm <span class="poppins text-violet-400">Alex Ferguson</span>
        <br />Full Stack
        <span class="poppins text-violet-400">Developer</span>
      </h2>
      <p class="text-base sm:text-lg md:text-xl">
        My <span class="text-violet-400">favourite tech</span> includes JavaScript,
        Python, Java, Node.js + Express.js & MongoDB!
      </p>
    </div>
  </section>

  <section
    id="about"
    class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
  >
    <div
      class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
    >
      <h6 class="text-large sm:text-xl md:text-2xl">Want to know more?</h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        A bit <span class="poppins text-violet-400">about</span> me.
      </h3>
    </div>
    <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
      I am . . .
    </p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
      {#each benefits as benefit, index}
        <div class="flex gap-6 sm:gap-8">
          <p
            class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
          >
            0{index + 1}
          </p>
          <div class="flex flex-col gap-6 sm:gap-8">
            <h3 class="text-2xl sm:text-3xl md:text-5xl">
              {benefit.name}
            </h3>
            <ul>
              {@html benefit.description}
            </ul>
          </div>
        </div>
      {/each}
    </div>

    <div
      class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
    />
  </section>
</main>
