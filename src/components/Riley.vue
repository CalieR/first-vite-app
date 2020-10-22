<template>
  
 <header>
      <h1>{{ msg }}!</h1>
    </header>
    <section id="main">
      <article>
        <img src="src/assets/Riley01.jpg" style="width: 500px" />
      </article>
      <aside>
        <h2>a.k.a</h2>
        <div v-for="nickname in nicknames">
          <p>{{ nickname }}</p>
        </div>
      </aside>
    </section>
    <footer>
      <p>powered by facelicks 🐶</p>
    </footer>
</template>

<script>
export default {
  name: 'Riley',
  props: {
    msg: String
  },
  data() {
    return {
      nicknames: [
      "Dizbot 3000",
      "R-Dizzle",
      "Mr Fluffkins",
      "Snuzz-Lord",
      "Monster Truck",
      "Riley Bear",
      "Grump Lord"
    ],
    }
  }
}
</script>
