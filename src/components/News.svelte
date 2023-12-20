<script>
  let items = [
    {
      id: 1,
      username: 'Queaxtra',
      avatar: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186752281257976010/avatarimage_1.png?ex=65946430&is=6581ef30&hm=38841404823f22342b2f37d9a20c11b3d22d35cc8736cdb4accc184eb9e3cafd&',
      image: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186753106374049973/Adsz_tasarm.png?ex=659464f5&is=6581eff5&hm=4b741d0a02560d0b444dfb91338dc3b3ef4efde31e6660fe324834c5433927b1&',
      title: 'News Title',
      tags: ["#Tag 1", "#Tag 2"]
    },
    {
      id: 2,
      username: 'guruıshackoy',
      avatar: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186752281257976010/avatarimage_1.png?ex=65946430&is=6581ef30&hm=38841404823f22342b2f37d9a20c11b3d22d35cc8736cdb4accc184eb9e3cafd&',
      image: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186753106374049973/Adsz_tasarm.png?ex=659464f5&is=6581eff5&hm=4b741d0a02560d0b444dfb91338dc3b3ef4efde31e6660fe324834c5433927b1&',
      title: 'News Title',
      tags: ["#Tag 1", "#Tag 2"]
    },
    {
      id: 3,
      username: 'boundizm',
      avatar: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186752281257976010/avatarimage_1.png?ex=65946430&is=6581ef30&hm=38841404823f22342b2f37d9a20c11b3d22d35cc8736cdb4accc184eb9e3cafd&',
      image: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186753106374049973/Adsz_tasarm.png?ex=659464f5&is=6581eff5&hm=4b741d0a02560d0b444dfb91338dc3b3ef4efde31e6660fe324834c5433927b1&',
      title: 'News Title',
      tags: ["#Tag 1", "#Tag 2"]
    },
    {
      id: 4,
      username: 'ataraksiya',
      avatar: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186752281257976010/avatarimage_1.png?ex=65946430&is=6581ef30&hm=38841404823f22342b2f37d9a20c11b3d22d35cc8736cdb4accc184eb9e3cafd&',
      image: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186753106374049973/Adsz_tasarm.png?ex=659464f5&is=6581eff5&hm=4b741d0a02560d0b444dfb91338dc3b3ef4efde31e6660fe324834c5433927b1&',
      title: 'News Title',
      tags: ["#Tag 1", "#Tag 2"]
    },
    {
      id: 5,
      username: 'h4dean',
      avatar: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186752281257976010/avatarimage_1.png?ex=65946430&is=6581ef30&hm=38841404823f22342b2f37d9a20c11b3d22d35cc8736cdb4accc184eb9e3cafd&',
      image: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186753106374049973/Adsz_tasarm.png?ex=659464f5&is=6581eff5&hm=4b741d0a02560d0b444dfb91338dc3b3ef4efde31e6660fe324834c5433927b1&',
      title: 'News Title',
      tags: ["#Tag 1", "#Tag 2"]
    },
    {
      id: 6,
      username: 'axeos',
      avatar: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186752281257976010/avatarimage_1.png?ex=65946430&is=6581ef30&hm=38841404823f22342b2f37d9a20c11b3d22d35cc8736cdb4accc184eb9e3cafd&',
      image: 'https://cdn.discordapp.com/attachments/1136591322208272385/1186753106374049973/Adsz_tasarm.png?ex=659464f5&is=6581eff5&hm=4b741d0a02560d0b444dfb91338dc3b3ef4efde31e6660fe324834c5433927b1&',
      title: 'News Title',
      tags: ["#Tag 1", "#Tag 2"]
    },
  ];
</script>

<div class="relative">
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 xl:grid-cols-5 gap-4 m-5 mx-12 md:mx-10 lg:mx-10 mt-32 md:mt-52 lg:mt-52">
    {#each items as item (item.id)}
      <div class="w-80 h-72 bg-white rounded drop-shadow-md">
        <section class="w-auto h-16 bg-[#e7e7e7] rounded-t-lg transition-all duration-300">
          <div class="float-right">
            <img class="w-10 bg-[#B0CB4D] rounded-full mx-3 my-2.5" src={item.avatar} alt="">
          </div>
          <h1 class="text-black absolute m-5">{item.username}</h1>
        </section>

        <div class="bg-[#B0CB4D] p-2">
          <img class="rounded h-20" src={item.image} alt="">
        </div>

        <div class="m-2">
          <h1 class="text-black text-lg">{item.title}</h1>
          <a href="/" class="text-black text-sm underline">
            <i class="fa-solid fa-arrow-up-right-from-square"></i> Haberi görüntüle
          </a>
        </div>

        <div class="m-2">
          {#each item.tags as tag (tag)}
            <span class="bg-blue-500 p-1 px-3 rounded-full text-xs mx-1 relative -left-1">{tag}</span>
          {/each}
        </div>
      </div>
    {/each}
  </div>
</div>