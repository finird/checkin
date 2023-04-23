<template>
  <div class="flex flex-col items-center justity-center">
    <h1>
      Personal user page {{userId}}
    </h1>
    <h2>Thong tin chi tiet...</h2>
    <button type="submit"
            class="flex w-[300px] justify-center rounded-md bg-indigo-600 px-3 py-1.5 text-sm font-semibold leading-6 text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
            @click="checkinAndGoBack"
    >Confirm</button>
  </div>
</template>

<script setup>

const route = useRoute();
const router = useRouter();

const userId = route.params.id;

const checkinAndGoBack = () => {
  alert('Checkin succeed!');
  router.replace('/dashboard');
}

</script>