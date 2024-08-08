<script lang="ts">
import NavBar from "../components/NavBar.svelte";
import Home from '../../assets/Home.svg';
import Logo from '../../assets/Books.svg';
import {Link} from 'svelte-routing';
</script>


<body class="bg-cover bg-no-repeat flex flex-col min-h-screen" style="background-image: url({Home});">
  <NavBar />
  <main class="flex-grow flex flex-col justify-center items-center w-4/5 h-auto mx-auto my-10 bg-gray-900 p-10 shadow-xl rounded-xl">
    <div class="flex flex-shrink-0 items-center">
      <img class="h-8 w-auto" src={Logo} alt="Your Company">
      <span class=" font-bold text-4xl ml-3 bg-gradient-to-r from-blue-500 to-purple-500 bg-clip-text text-transparent"> RevisionTutor </span>
    </div>
    <hr class="my-2">
    <p class="text-left text-lg leading-relaxed mb-5 text-white">
      Welcome to Revision Tutor, the ultimate community for International General Certificate of Secondary Education (IGCSE) students! Here, you'll find a vast collection of revision notes and past papers tailored to help you excel in your studies. Our platform is designed to make learning more interactive and accessible, allowing you to upload your own study materials, search for specific topics, and collaborate with fellow students. Whether you're preparing for upcoming exams or seeking additional resources to reinforce your understanding, Revision Tutor is your go-to hub for all things IGCSE. Join us today and take the first step towards achieving academic success!
    </p>
    <Link class="Start_button mt-5 px-5 py-2 bg-gradient-to-r from-blue-500 to-purple-500 text-white rounded-md hover:bg-green-700" to="/search">
      Start Learning
    </Link>
  </main>
  <footer class="text-center p-3 bg-gray-900 w-full text-white">
    &copy; 2024
  </footer>
</body>
