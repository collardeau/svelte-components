<script>
  import Headroom from "./index.svelte";

  const onPin = () => {
    console.log("pin");
  };
</script>

<style>
  header {
    background-color: darkblue;
    height: 60px;
  }
  main {
    padding-top: 60px;
    height: 150vh; /* enough room to scroll */
  }
  p {
    padding: 0 1rem;
  }
</style>

<Headroom on:pin={onPin} duration="350ms" offset={50} tolerance={5}>
  <header />
</Headroom>

<main>
  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Id sequi
    distinctio, eveniet non mollitia ea asperiores laborum excepturi modi ut
    similique amet, ducimus facilis atque? Iure, distinctio, atque odit nisi
    maxime aliquid quam incidunt earum magnam vel quia accusantium numquam. Quo
    magni id excepturi repellendus eum quibusdam maxime blanditiis commodi
    inventore reiciendis? Dolor eum voluptatem facere libero ipsam et
    consectetur saepe, magni cupiditate dolore quis laborum optio corporis cum
    similique eos quae vel mollitia neque! Consequatur dolorum magnam assumenda
    distinctio, fuga voluptates. Fugiat, adipisci aliquid reiciendis repellat
    possimus aut rem excepturi, quae odio laboriosam voluptas. Quidem tempore
    porro officia placeat in consequuntur earum aliquam ad error nostrum ab
    incidunt doloremque suscipit ipsa odio veritatis fuga voluptate, dolor,
    molestias quam aperiam accusantium. Laboriosam mollitia laborum, quibusdam
    praesentium dicta vero, quas quam necessitatibus optio impedit recusandae
    perferendis sunt consequatur? Magnam minus perspiciatis deserunt rerum
    necessitatibus in nobis ipsum animi delectus! Fuga, repellendus architecto
    quam, cum quae perferendis eos dicta repellat sequi, sapiente voluptatibus
    magnam incidunt. Totam incidunt ipsa ipsam laboriosam nostrum aspernatur
    voluptatum impedit atque, harum, ab reprehenderit omnis aliquam magni minima
    dolorum eius, saepe corrupti illum dicta quis facere sint perferendis.
    Tenetur beatae tempora inventore voluptatibus consequuntur voluptas
    molestiae, quo reiciendis quisquam, placeat odit! Dolores, obcaecati dolor.
    Non enim impedit, mollitia deleniti dicta quaerat ipsam, ea beatae id,
    repellat ullam repudiandae vel? Veniam laboriosam sequi facere voluptate
    placeat, rem non dolores optio commodi quod porro voluptatibus
    exercitationem ea voluptatem quae earum dicta velit maiores sint modi
    voluptates molestiae ipsam, quam pariatur. Eum saepe quas commodi minima
    asperiores eius ipsam deleniti voluptatem voluptas qui, unde facilis
    numquam, illo et ullam ex ipsa voluptatibus. Suscipit illum et recusandae
    deserunt, accusantium, quo qui dolore fuga voluptatibus quam ex! Accusamus
    quod praesentium sint labore debitis iure nostrum harum alias! Suscipit
    dignissimos, amet fuga nam consequuntur quia libero consectetur omnis dolore
    obcaecati velit ad vel voluptates saepe! Eius accusamus incidunt labore et
    excepturi facere adipisci, odio pariatur, soluta consequatur voluptates
    deleniti ex at ut dolore nihil velit facilis quam distinctio consequuntur
    quis neque architecto? Quasi adipisci omnis debitis impedit dolores, sint
    harum ipsum cumque dolorem possimus maiores quis iste mollitia ratione
    aperiam optio sed, atque voluptate soluta enim beatae et. Provident deleniti
    cum praesentium libero dolor, mollitia totam accusamus doloremque tempora
    itaque quisquam nostrum earum quam excepturi sequi accusantium autem velit
    hic pariatur deserunt ullam vel possimus! Sequi, quae dolorem voluptas
    exercitationem quibusdam odit pariatur, tempore iste nam quo, illo totam
    placeat porro ut et vel similique ex reiciendis doloremque nostrum maxime
    rerum? Repellendus quam aut modi maiores voluptas reiciendis similique
    facere nulla quibusdam, dolor architecto deleniti velit perferendis aliquam
    nemo, expedita cumque! Nesciunt veniam animi officia, provident illo commodi
    iure sequi omnis facere corrupti voluptas reiciendis cupiditate numquam
    excepturi nobis. Architecto officiis ut dicta? Alias provident in, expedita
    similique debitis, nobis aliquid totam porro, est assumenda ex modi ab
    perferendis deleniti numquam quia repellat laboriosam. Expedita, harum ea
    cupiditate vel omnis placeat distinctio reprehenderit! Dolorum inventore
    quaerat voluptatibus illum itaque ipsum, explicabo ipsa nihil porro.
  </p>
  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Id sequi
    distinctio, eveniet non mollitia ea asperiores laborum excepturi modi ut
    similique amet, ducimus facilis atque? Iure, distinctio, atque odit nisi
    maxime aliquid quam incidunt earum magnam vel quia accusantium numquam. Quo
    magni id excepturi repellendus eum quibusdam maxime blanditiis commodi
    inventore reiciendis? Dolor eum voluptatem facere libero ipsam et
    consectetur saepe, magni cupiditate dolore quis laborum optio corporis cum
    similique eos quae vel mollitia neque! Consequatur dolorum magnam assumenda
    distinctio, fuga voluptates. Fugiat, adipisci aliquid reiciendis repellat
    possimus aut rem excepturi, quae odio laboriosam voluptas. Quidem tempore
    porro officia placeat in consequuntur earum aliquam ad error nostrum ab
    incidunt doloremque suscipit ipsa odio veritatis fuga voluptate, dolor,
    molestias quam aperiam accusantium. Laboriosam mollitia laborum, quibusdam
    praesentium dicta vero, quas quam necessitatibus optio impedit recusandae
    perferendis sunt consequatur? Magnam minus perspiciatis deserunt rerum
    necessitatibus in nobis ipsum animi delectus! Fuga, repellendus architecto
    quam, cum quae perferendis eos dicta repellat sequi, sapiente voluptatibus
    magnam incidunt. Totam incidunt ipsa ipsam laboriosam nostrum aspernatur
    voluptatum impedit atque, harum, ab reprehenderit omnis aliquam magni minima
    dolorum eius, saepe corrupti illum dicta quis facere sint perferendis.
    Tenetur beatae tempora inventore voluptatibus consequuntur voluptas
    molestiae, quo reiciendis quisquam, placeat odit! Dolores, obcaecati dolor.
    Non enim impedit, mollitia deleniti dicta quaerat ipsam, ea beatae id,
    repellat ullam repudiandae vel? Veniam laboriosam sequi facere voluptate
    placeat, rem non dolores optio commodi quod porro voluptatibus
    exercitationem ea voluptatem quae earum dicta velit maiores sint modi
    voluptates molestiae ipsam, quam pariatur. Eum saepe quas commodi minima
    asperiores eius ipsam deleniti voluptatem voluptas qui, unde facilis
    numquam, illo et ullam ex ipsa voluptatibus. Suscipit illum et recusandae
    deserunt, accusantium, quo qui dolore fuga voluptatibus quam ex! Accusamus
    quod praesentium sint labore debitis iure nostrum harum alias! Suscipit
    dignissimos, amet fuga nam consequuntur quia libero consectetur omnis dolore
    obcaecati velit ad vel voluptates saepe! Eius accusamus incidunt labore et
    excepturi facere adipisci, odio pariatur, soluta consequatur voluptates
    deleniti ex at ut dolore nihil velit facilis quam distinctio consequuntur
    quis neque architecto? Quasi adipisci omnis debitis impedit dolores, sint
    harum ipsum cumque dolorem possimus maiores quis iste mollitia ratione
    aperiam optio sed, atque voluptate soluta enim beatae et. Provident deleniti
    cum praesentium libero dolor, mollitia totam accusamus doloremque tempora
    itaque quisquam nostrum earum quam excepturi sequi accusantium autem velit
    hic pariatur deserunt ullam vel possimus! Sequi, quae dolorem voluptas
    exercitationem quibusdam odit pariatur, tempore iste nam quo, illo totam
    placeat porro ut et vel similique ex reiciendis doloremque nostrum maxime
    rerum? Repellendus quam aut modi maiores voluptas reiciendis similique
    facere nulla quibusdam, dolor architecto deleniti velit perferendis aliquam
    nemo, expedita cumque! Nesciunt veniam animi officia, provident illo commodi
    iure sequi omnis facere corrupti voluptas reiciendis cupiditate numquam
    excepturi nobis. Architecto officiis ut dicta? Alias provident in, expedita
    similique debitis, nobis aliquid totam porro, est assumenda ex modi ab
    perferendis deleniti numquam quia repellat laboriosam. Expedita, harum ea
    cupiditate vel omnis placeat distinctio reprehenderit! Dolorum inventore
    quaerat voluptatibus illum itaque ipsum, explicabo ipsa nihil porro.
  </p>
</main>
