<script>
  let developers = [
    {
      name: 'Genta putra harnaci',
      status: 'Alumni 2021',
    },
    {
      name: 'Desal Isra',
      status: 'Alumni 2017',
    },
    {
      name: 'M Miftahurrahman',
      status: 'Active',
    },
    {
      name: 'Romadoni Eko Putro',
      status: 'Active',
    },
    {
      name: 'Muhammad Riza Putra',
      status: 'Active',
    },
    {
      name: 'Stefanie',
      status: 'Active',
    },
    {
      name: 'Satrio Arum Wijaya K',
      status: 'Active',
    },
    {
      name: 'Aldi Sunantri',
      status: 'Active',
    },
    {
      name: 'Alfiyan Nugroho',
      status: 'Active',
    },
    {
      name: 'Siti Aulia Jasmine',
      status: 'Active',
    },
    {
      name: 'Dewi Susan Suriani',
      status: 'Active',
    },
    {
      name: 'Rizky Oktaviani',
      status: 'Active',
    },
    {
      name: 'Aida Ainun Najah',
      status: 'Active',
    },
    {
      name: 'Rizky Ananda',
      status: 'Active',
    },
    {
      name: 'Fadilah Permana',
      status: 'Active',
    },
    {
      name: 'M Aldi Pratama',
      status: 'Active',
    },
    {
      name: 'Muhammad Ariel',
      status: 'Active',
    },
    {
      name: 'M Anton Fahrdzzi',
      status: 'Active',
    },
    {
      name: 'Ardhi Anggoro',
      status: 'Active',
    },
    {
      name: 'Wahyu Setyo Budi Utomo',
      status: 'Active',
    },
    {
      name: 'M Farhan',
      status: 'Active',
    },
    {
      name: 'M Akbar Febriyan',
      status: 'Active',
    },
    {
      name: 'Azhar Rifal',
      status: 'Active',
    },
    {
      name: 'Gunawan',
      status: 'Active',
    },
    {
      name: 'Dadan Ramadhan',
      status: 'Active',
    },
  ];
</script>

<nav
  class="fixed top-0 w-full h-11 flex justify-between items-center px-6 shadow-md text-sm bg-white"
  style="box-shadow: 0px 2px 2px rgb(0 0 0 / 5%);"
>
  <div class="flex gap-3 items-center">
    <img
      src="https://assets.smkymik.sch.id/images/logo/main.png"
      alt=""
      class="w-6"
    />
    <h3>Developers</h3>
  </div>
  <div class="flex gap-3 ">
    <a href="#about">About</a>
    <a href="#project">Project</a>
    <a href="#team">Team</a>
  </div>
</nav>
<img
  src="https://assets.smkymik.sch.id/images/undraw/developer_activity.svg"
  alt=""
  class="absolute  w-72 -right-52 md:-right-28 top-44 -z-50 "
/>
<main
  id="about"
  class="flex justify-center items-center text-center mt-16 pt-16 "
>
  <div class="text-center">
    <h1 class="text-4xl font-bold mb-4">
      SMK YMIK <span class="text-primary">DEVELOPERS</span>
    </h1>
    <p class="text-sm max-w-sm leading-6  p-6">
      Mari Bergabung untuk belajar bersama serta berikan kontribusi anda disini
    </p>
    <a
      href="https://github.com/smk-ymik"
      target="_blank"
      class="bg-primary px-4 py-2 rounded-full text-white text-sm hover:shadow-md transition-shadow"
    >
      Lihat Github
    </a>
  </div>
</main>
<section id="project" class="mt-10 p-10">
  <h2 class="font-bold text-xl mb-10">Apa yang sudah kami buat</h2>
  <div class="flex gap-6 flex-wrap ">
    {#each [1] as { }}
      <div
        class="border max-w-xs py-4 px-6 rounded-2xl bg-white hover:text-white hover:bg-primary cursor-pointer transition-colors"
      >
        <div class="flex text-xs justify-between mb-4">
          <span>Website</span>
          <span>18 Juni 2022</span>
        </div>
        <h3 class="font-medium mb-4">Web Protofolio</h3>
        <p class="text-sm">
          Sebuah website yang menampilkan data personal sesorang
        </p>
        <div class="flex justify-end ">
          <a href="#">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="icon icon-tabler icon-tabler-arrow-right"
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
              <line x1="5" y1="12" x2="19" y2="12" />
              <line x1="13" y1="18" x2="19" y2="12" />
              <line x1="13" y1="6" x2="19" y2="12" />
            </svg>
          </a>
        </div>
      </div>
    {/each}
  </div>
</section>
<img
  src="https://assets.smkymik.sch.id/images/undraw/rocket.svg"
  alt=""
  class="absolute  w-72  -left-32 sm:-left-28 top-[30rem] -z-50 "
/>
<section id="team" class="mt-10 p-10">
  <h2 class="font-bold text-xl mb-10 text-center">
    Mari Berkenalan dengan para developer
  </h2>
  <div class="flex gap-6 flex-wrap justify-center items-center ">
    {#each developers as { name, status }}
      <div
        class="border w-80 py-4 px-6 rounded-md bg-white flex gap-3 hover:shadow-md transition-shadow cursor-pointer"
      >
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
    {/each}
  </div>
</section>
<img
  src="https://assets.smkymik.sch.id/images/undraw/team.svg"
  alt=""
  class="absolute  w-72 -right-36 md:-right-32 top-[70rem]  md:top-[45rem] -z-50 "
/>
<footer class="text-center mb-3 text-sm">
  <p>Hak Cipta 2022 Oleh Para Developer SMK YMIK</p>
</footer>

<style>
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>
