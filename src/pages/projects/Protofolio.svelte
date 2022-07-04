<script>
  import Navbar from '../../components/Navbar.svelte';
  import { Swipe, SwipeItem } from 'svelte-swipe';

  const swipeConfig = {
    autoplay: false,
    delay: 2000,
    transitionDuration: 1000,
    defaultIndex: 0,
  };

  let developers = [
    {
      name: 'Genta putra harnaci',
      status: 'Alumni 2021',
    },
    {
      name: 'Desal Isra',
      status: 'Alumni 2017',
    },
  ];
</script>

<Navbar />

<main class="w-10/12 mx-auto">
  <div class="w-full h-20 mx-auto my-10 border rounded-md">
    <Swipe {...swipeConfig}>
      {#each developers as { name, status }}
        <SwipeItem>
          <div
            class=" p-4 max-w-full  rounded-md bg-white flex justify-between gap-3 items-center hover:shadow-md transition-shadow cursor-pointer"
          >
            <div class="flex gap-3">
              <div
                class="border w-10 h-10 rounded-full bg-primary flex justify-center items-center font-bold text-white"
              >
                <span>{name.charAt(0)}</span>
              </div>
              <div>
                <h3 class="font-semibold capitalize">{name}</h3>
                <p class="text-xs capitalize">{status}</p>
              </div>
            </div>
            <a href="#" class="text-primary">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="icon icon-tabler icon-tabler-browser-plus"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                stroke-width="2"
                stroke="currentColor"
                fill="none"
                stroke-linecap="round"
                stroke-linejoin="round"
              >
                <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                <rect x="4" y="4" width="16" height="16" rx="1" />
                <path d="M4 8h16" />
                <path d="M8 4v4" />
                <path d="M10 14h4" />
                <path d="M12 12v4" />
              </svg>
            </a>
          </div>
        </SwipeItem>
      {/each}
    </Swipe>
  </div>

  <iframe
    title="Protofolio"
    src="https://developers.smkymik.sch.id/projects/protofolio/miftah.html"
    frameborder="0"
    class=" w-full mx-auto border shadow-sm h-[35rem] overflow-hidden"
  />
</main>
