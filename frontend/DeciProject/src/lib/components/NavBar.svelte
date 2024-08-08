<script lang="ts">
    import Logo from "../../assets/Books.svg";
    import {Link} from "svelte-routing";
</script>

<nav class="bg-gray-950">
    <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
      <div class="relative flex h-20 items-center justify-between">
        <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
          <div class="flex flex-shrink-0 items-center">
            <img class="h-8 w-auto" src={Logo} alt="Your Company">
            <span class="text-white font-bold text-xl ml-3"> RevisionTutor </span>
          </div>
          <div class="hidden sm:ml-6 sm:block">
            <div class="flex space-x-4">
              <Link to="/" class="px-5 py-2 text-base font-medium text-gray-300 hover:border-0 hover:border-purple-500 hover:border-b-2" aria-current="page">Home</Link>
              <Link to="/search" class="px-5 py-2 text-base font-medium text-gray-300 hover:border-0 hover:border-purple-500 hover:border-b-2">Access Notes</Link>
              <Link to="/upload" class="px-5 py-2 text-base font-medium text-gray-300 hover:border-0 hover:border-purple-500 hover:border-b-2">Upload Notes</Link>
              <Link to="/about" class="px-5 py-2 text-base font-medium text-gray-300 hover:border-0 hover:border-purple-500 hover:border-b-2">About Us</Link>
            </div>
          </div>
        </div>
        <div class="absolute inset-y-0 right-0 flex items-center pr-2">
          <button type="button" class="bg-purple-500 rounded-xl px-5 py-2  text-white hover:rounded-3xl hover:px-6 transition-all ease-in duration-100">
            Sign In
          </button>
        </div>
      </div>
    </div>
</nav>
  