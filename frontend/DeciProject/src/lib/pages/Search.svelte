<script lang="ts">
  import NavBar from "../components/NavBar.svelte";
  import SearchBar from "../components/SearchBar.svelte";
  import Background from "../../assets/Background.svg";
  import Toggle from "../components/Toggle.svelte";
</script>

<NavBar />
<body class="bg-gray-800">
  <div class="w-auto pt-10 mb-10">
    <p class="my-14 text-5xl font-bold text-center bg-gradient-to-r from-blue-500 to-red-500 bg-clip-text text-transparent"> A World of Resources is Just a Few Clicks Away  </p>
    <SearchBar />
  </div>

  <div class="flex justify-between items-center text-white font-semibold text-xl">
    <div class="mx-8 px-6 py-3 flex-grow text-center">
      Subject Level
      <hr class="bg-gradient-to-r from-blue-600 to-purple-600 h-1 border-none rounded-full my-2">
      <fieldset class="mt-4 border p-5 rounded-xl ">

        <div class="flex items-center mb-4">
          <Toggle text="IGCSE"/>
        </div>

        <div class="flex items-center mb-4">
          <Toggle text="GCSE"/>
        </div>

        <div class="flex items-center mb-4">
          <Toggle text="AS Level"/>
        </div>

        <div class="flex items-center mb-4">
          <Toggle text="A2 Level"/>
        </div>

      
  
      </fieldset>

    </div>
    <div class="mx-8 px-6 py-3 flex-grow text-center"> 
      Exam Board
      <hr class="bg-gradient-to-r from-blue-600 to-purple-600 h-1 border-none rounded-full my-2">
      <fieldset class="mt-4 border p-5 rounded-xl ">

        <div class="flex items-center mb-4">
          <Toggle text="Cambridge"/>
        </div>

        <div class="flex items-center mb-4">
          <Toggle text="Edexcel"/>
        </div>

        <div class="flex items-center mb-4">
          <Toggle text="Oxford"/>
        </div>

        <div class="flex items-center mb-4">
          <Toggle text="Welsh Joint Education Committee"/>
        </div>
      </fieldset>
    </div>
    <div class="mx-8 px-6 py-3 flex-grow text-center"> 
      Resource Type
      <hr class="bg-gradient-to-r from-blue-600 to-purple-600 h-1 border-none rounded-full my-2">
      <fieldset class="mt-4 border p-5 rounded-xl ">

        <div class="flex items-center mb-4">
          <Toggle text="Images/Scanned Notes"/>
        </div>

        <div class="flex items-center mb-4">
          <Toggle text="Word Document/PDF Files"/>
        </div>

        <div class="flex items-center mb-4">
          <Toggle text="Videos/Animations"/>
        </div>

        <div class="flex items-center mb-4">
          <Toggle text="Pictures"/>
        </div>

      
  
      </fieldset>


    </div>
  </div>
</body>