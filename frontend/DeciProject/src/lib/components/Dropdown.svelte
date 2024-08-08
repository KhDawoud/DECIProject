<script lang="ts">
    export let options;
    export let text;
</script>

<div class="">
    <label for="category" class="block mb-2 text-base font-semibold text-white">{text}</label>
    <select id="category" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-primary-500 focus:border-primary-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500">
        <option selected> Select a {text} </option>
        {#each options as option}
        <option> {option} </option>
        {/each}
    </select>
  </div>