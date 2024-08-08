<script lang="ts">
  import Dropdown from "../components/Dropdown.svelte";
import NavBar from "../components/NavBar.svelte";


</script>

<body class="bg-custom-bg bg-cover bg-center min-h-screen">
  <NavBar />
  <div class="flex items-center justify-center min-h-screen">
    <main class="border border-cyan-500 shadow-xl rounded-xl w-3/4 bg-gray-900 p-8 px-12 min-h-[30rem]">
      <header class="text-center text-4xl font-bold text-white">
        <h1> Please Enter Your Information</h1>
      </header>
      <hr class="my-3 bg-gradient-to-r from-blue-600 to-purple-600 h-1 border-none rounded-full ">
      <form class="text-white font-semibold h-[26rem] mx-5 space-y-5"> 
        <label class="bg-gray-900 text-gray-300 font-semibold text-base rounded min-w-sm h-36 flex flex-col items-center justify-center cursor-pointer border-2 border-gray-300 border-dashed font-[sans-serif]">
          <div class="flex items-center">
            <svg xmlns="http://www.w3.org/2000/svg" class="w-11 fill-gray-300 mr-2" viewBox="0 0 32 32">
              <path d="M23.75 11.044a7.99 7.99 0 0 0-15.5-.009A8 8 0 0 0 9 27h3a1 1 0 0 0 0-2H9a6 6 0 0 1-.035-12 1.038 1.038 0 0 0 1.1-.854 5.991 5.991 0 0 1 11.862 0A1.08 1.08 0 0 0 23 13a6 6 0 0 1 0 12h-3a1 1 0 0 0 0 2h3a8 8 0 0 0 .75-15.956z" data-original="#000000" />
              <path d="M20.293 19.707a1 1 0 0 0 1.414-1.414l-5-5a1 1 0 0 0-1.414 0l-5 5a1 1 0 0 0 1.414 1.414L15 16.414V29a1 1 0 0 0 2 0V16.414z" data-original="#000000" />
            </svg>
            <span>Upload file</span>
          </div>
          <input type="file" class="hidden" id="uploadFile1" />
          <p class="text-xs font-medium text-gray-200 mt-2">MP4, PDF, DOCX, JPG, and PNG are Allowed.</p>
        </label>
        <div class="grid grid-flow-col grid-cols-2 space-x-3">
          <Dropdown options={["Maths", "Chemistry", "Physics", "Biology", "English", "Business", "Geography", "History"]} text="Subject"/>
        <Dropdown text="Exam Board" options={["Cambridge", "Edexcel", "Oxford", "WJEC"]} />
        </div>
        
        <h3 class="mb-4 font-semibold text-white">Education Level</h3>
        <ul class="items-center w-full text-sm font-medium text-gray-900 bg-white border border-gray-200 rounded-lg sm:flex dark:bg-gray-700 dark:border-gray-600 dark:text-white">
            <li class="w-full border-b border-gray-200 sm:border-b-0 sm:border-r dark:border-gray-600">
                <div class="flex items-center ps-3">
                    <input type="checkbox" value="" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-700 dark:focus:ring-offset-gray-700 focus:ring-2 dark:bg-gray-600 dark:border-gray-500">
                    <label class="w-full py-3 ms-2 text-sm font-medium text-gray-300">IGCSE</label>
                </div>
            </li>
            <li class="w-full border-b border-gray-200 sm:border-b-0 sm:border-r dark:border-gray-600">
                <div class="flex items-center ps-3">
                    <input type="checkbox" value="" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-700 dark:focus:ring-offset-gray-700 focus:ring-2 dark:bg-gray-600 dark:border-gray-500">
                    <label  class="w-full py-3 ms-2 text-sm font-medium text-gray-300">AS Level</label>
                </div>
            </li>
            <li class="w-full border-b border-gray-200 sm:border-b-0 sm:border-r dark:border-gray-600">
                <div class="flex items-center ps-3">
                    <input id="angular-checkbox-list" type="checkbox" value="" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-700 dark:focus:ring-offset-gray-700 focus:ring-2 dark:bg-gray-600 dark:border-gray-500">
                    <label for="angular-checkbox-list" class="w-full py-3 ms-2 text-sm font-medium text-gray-300">A2 Level</label>
                </div>
            </li>
            <li class="w-full dark:border-gray-600">
                <div class="flex items-center ps-3">
                    <input id="laravel-checkbox-list" type="checkbox" value="" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-600 dark:ring-offset-gray-700 dark:focus:ring-offset-gray-700 focus:ring-2 dark:bg-gray-600 dark:border-gray-500">
                    <label for="laravel-checkbox-list" class="w-full py-3 ms-2 text-sm font-mediumtext-gray-300">GCSE</label>
                </div>
            </li>
        </ul>
        <button type="submit" class="bg-gradient-to-r from-blue-500 to-purple-500 rounded-xl px-5 py-2 w-full text-white hover:rounded-3xl hover:px-6 transition-all ease-in duration-100"> Submit</button>
        
      
      </form>
    </main>
  </div>

  
</body>
