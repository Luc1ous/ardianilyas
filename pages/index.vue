<template>
  <Head>
    <Title>Luc1ous</Title>
  </Head>
  <!-- Hero -->
  <div class="w-full max-w-3xl mx-auto min-h-screen flex justify-center items-center">
    <div class="text-center container">
      <h1 class="text-5xl md:text-6xl font-semibold">Ardian Ilyas Fernanda</h1>
      <p class="mt-2 text-sm md:text-base text-gray-600 md:leading-loose">A human that have interest about Web Programming. Currently interesting in a backend field (<span class="text-red-600">Laravel</span> , <span class="text-green-600">Express.js</span>, and <span class="text-violet-600">Adonis.js</span>). FYI this website is build using Nuxt.js and Tailwind CSS tech. This year I'am {{ age }} years old.</p>
    </div>
  </div>

  <!-- Skills section -->
  <div class="container w-full min-h-screen p-10" id="skills">
    <h2 class="text-center font-semibold text-4xl">Skills</h2>
    <p class="text-center text-gray-600">There are my skills about web programming (programming language, software, etc).</p>

    <div class="my-8 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
      <a :href="skill.href" target="_blank" v-for="skill in skills" class="bg-white p-6 shadow-md rounded-md border border-gray-200 hover:bg-gray-50/70 flex flex-col justify-center">
        <h4 :class="skill.color" class="text-xl font-semibold">{{ skill.name }}</h4>
        <p class="mt-2 text-sm text-gray-600 leading-loose">{{ skill.description }}</p>
      </a>
    </div>
  </div>

  <!-- Github repo -->
  <div class="container w-full p-10 flex flex-col justify-center items-center">
    <img src="~/assets/img/github.png" width="50" alt="">
    <h2 class="mt-2 text-center text-3xl font-semibold">Kindly check my github repository <a href="https://github.com/Luc1ous" target="_blank" class="text-blue-600 underline underline-offset-4">here</a> </h2>
  </div>

  <div class="w-full bg-white/70 p-10 text-center">
    <p class="text-gray-600">&copy; {{ new Date().getFullYear() }} Ardian Ilyas Fernanda. All rights reserved.</p>
  </div>
</template>

<script setup>
  const age = new Date().getFullYear() - 2002
  const skills = [
    {
      name: "HTML",
      description: "HTML is the standard markup language for Web pages",
      color: 'text-orange-500',
      href: "https://html.com/"
    },
    {
      name: "CSS",
      description: "Cascading Style Sheets (CSS) is a stylesheet language used to describe the presentation of a document written in HTML or XML",
      color: "text-blue-600"
    },
    {
      name: "JavaScript",
      description: "JavaScript is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much",
      color: "text-yellow-400",
      href: "https://www.javascript.com/"
    },
    {
      name: "PHP",
      description: "PHP is a general-purpose scripting language geared towards web development.",
      color: "text-purple-900",
      href: "https://www.php.net/"
    },
    {
      name: "Bootstrap",
      description: "Bootstrap is a free front-end framework for faster and easier web development",
      color: "text-indigo-700",
      href: "https://getbootstrap.com/"
    },
    {
      name: "Tailwind CSS",
      description: "Tailwind CSS is a utility-first CSS framework for rapidly building modern websites without ever leaving your HTML.",
      color: "text-cyan-400",
      href: "https://tailwindcss.com/"
    },
    {
      name: "Vue.js",
      description: "The Progressive JavaScript Framework",
      color: "text-emerald-600",
      href: "https://vuejs.org/"
    },
    {
      name: "Nuxt.js",
      description: "Nuxt is an open source framework that makes web development intuitive and powerful",
      color: "text-green-500",
      href: "https://nuxt.com/"
    },
    {
      name: "React.js",
      description: "React is the library for web and native user interfaces",
      color: "text-sky-600",
      href: "https://react.dev/"
    },
    {
      name: "Next.js",
      description: "Next.js is a flexible React framework that gives you building blocks to create fast, full-stack web applications",
      href: "https://nextjs.org/"
    },
    {
      name: "Node.js",
      description: "Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine",
      color: "text-green-800",
      href: "https://nodejs.org/en"
    },
    {
      name: "Express.js",
      description: "Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications",
      href: "https://expressjs.com/"
    },
    {
      name: "Laravel",
      description: "Laravel is a PHP web application framework with expressive, elegant syntax",
      color: "text-red-600",
      href: "https://laravel.com/"
    },
    {
      name: "Livewire",
      description: "A full-stack framework for Laravel that takes the pain out of building dynamic UIs",
      color: "text-pink-600",
      href: "https://livewire.laravel.com/"
    },
    {
      name: "Inertia.js",
      description: "Inertia allows you to create fully client-side rendered, single-page apps, without the complexity that comes with modern SPAs",
      color: "text-purple-500",
      href: "https://inertiajs.com/"
    },
    {
      name: "MySQL",
      description: "MySQL is a widely used relational database management system (RDBMS)",
      color: "text-blue-900",
      href: "https://www.mysql.com/"
    },
    {
      name: "MongoDB",
      description: "MongoDB is an open source NoSQL database management program",
      color: "text-green-900",
      href: "https://www.mongodb.com/"
    },
    {
      name: "Figma",
      description: "Figma is the leading collaborative design tool for building meaningful products",
      color: "text-orange-600",
      href: "https://www.figma.com/"
    },
  ]
</script>

<style lang="scss" scoped>

</style>