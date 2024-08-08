<script lang="ts">
  import NavBar from "../components/NavBar.svelte";
  import GroupImage from "../../assets/GroupImage.jpg";
  import Background from "../../assets/AboutUs.svg"
</script>

<body class="font-sans m-0 p-0 box-borderbg-no-repeat bg-cover flex flex-col" style="background-image: url({Background});">
  <NavBar />
  <main class="max-w-4xl mx-auto my-10 p-8 bg-gray-900 shadow-lg rounded-xl flex flex-col items-center text-center">
    <h1 class="text-6xl my-5 font-bold mb-2 bg-gradient-to-r from-blue-500 to-red-500 bg-clip-text text-transparent">About Us</h1>
    <img src={GroupImage} alt="" class="max-w-full h-auto my-5 rounded-xl">
    <p class="mb-5 text-justify text-gray-200">
      Certainly! Here’s a more detailed version:

Welcome to our dedicated hub for IG students, designed with the goal of streamlining your study process and enhancing collaboration. Our platform is the result of a group project for the DECI scholarship, crafted by a team of passionate students: Khaled Dawoud, Youssef Hany, Amr Wael, and Hamza Moustafa. As part of our final project, we aimed to create a comprehensive resource where students can effortlessly upload, search for, and access valuable notes and revision papers.

Understanding the challenges faced by students in managing and sharing study materials, we built this site to facilitate easy communication and efficient study practices. Our mission is to provide a user-friendly space that supports academic success and fosters a community of learners who can help each other thrive. By bringing together essential study tools in one place, we hope to empower students to achieve their goals and succeed in their academic endeavors, just as we have strived to do through this project.
    </p>       
  </main>
  <footer class="text-center p-3 bg-gray-900 w-full text-white">
    &copy; 2024
  </footer>
</body>
