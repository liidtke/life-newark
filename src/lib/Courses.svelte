<script lang="ts">
  let header = {
    name: "Curso",
    prof: "Professor",
    period: "Período",
    age: "Idade",
    day: "Dia",
    value: "Valor",
    lang: "Idioma",
    contact: "Contato",
  };

  let items = [
    {
      name: "Violão",
      prof: "Richard Isaac",
      period: "Semestral",
      age: "Todas",
      day: "Segunda às 7pm",
      value: "$10",
      lang: "Português",
      contact: "(908) 342-3972",
    },
    {
      name: "Piano",
      prof: "Richard Isaac",
      period: "Semestral",
      age: "Todas",
      day: "Segunda às 8pm",
      value: "$10",
      lang: "Português",
      contact: "(908) 342-3972",
    },
    {
      name: "Canto",
      prof: "Marla Lüdtke",
      period: "Semestral",
      age: "Jovens e adultos",
      day: "Quarta às 6 pm",
      value: "$10",
      lang: "Português",
      contact: "(732) 209-0544",
    },
    {
      name: "Musicalização Infantil",
      prof: "Marla Lüdtke",
      period: "Semestral",
      age: "2 a 5 anos",
      day: "Quarta às 5 pm",
      value: "$10",
      lang: "Português",
      contact: "(732) 209-0544",
    },
    {
      name: "Coral de música popular brasileira (Parceria Mantena)",
      prof: "Daniel Lüdtke",
      period: "Anual",
      age: "Jovens e adultos",
      day: "Terças 7:30 pm",
      value: "Grátis",
      lang: "Português",
      contact: "(732) 209-0105",
    },
    {
      name: "Cursos para casais",
      prof: "Isabel Passos, Pablo Cisneros, Vivian Cisneros",
      period: "2 meses",
      age: "Casados",
      day: "Quintas às 8 pm",
      value: "$10 por casal",
      lang: "Português",
      contact: "(732) 209-0105",
    },
    {
      name: "Inglês para iniciantes",
      prof: "Roger Costa",
      period: "3 meses",
      age: "Jovens e adultos",
      day: "Quartas e quintas às 7:30 pm",
      value: "$10",
      lang: "Português e Inglês",
      contact: "(973) 745-8756",
    },
    {
      name: "Saúde mental, ansiedade e depressão",
      prof: "Joe Herrera",
      period: "2 meses",
      age: "Jovens e adultos",
      day: "Quartas às 7 pm",
      value: "$10",
      lang: "Espanhol e inglês",
      contact: "(646) 797-0408",
    },
  ];

  function open(phone:string){
    phone = phone.replace(/[^+\d]+/g, "");
    let formatted = '+1' +  phone;
    console.log(formatted)
    window.open('https://wa.me/' + formatted);
  }
</script>

<div class="p-strip">
  <div class="row">

    <p class="p-heading--1">Cursos</p>

    {#each items as item}

    <div class="p-card--highlighted">
      <div class="value">{item.value}</div>
      <h3><strong>
        {item.name}
      </strong>
      </h3>
      <p class="p-card__content">
        {header.prof}: {item.prof}
      </p>
      <p class="p-card__content">
        {header.period}: {item.period}
      </p>
      <p class="p-card__content">
        {header.age}: {item.age}
      </p>
      <p class="p-card__content">
        {header.day}: {item.day}
      </p>
      <!-- <p class="p-card__content">
        {header.value}: {item.value}
      </p> -->
      <p class="p-card__content">
        {header.lang}: {item.lang}
      </p>
      <p class="p-card__content">
        {header.contact}: <a href="tel:+1 {item.contact}">{item.contact}</a>
        <a on:click={() => open(item.contact)}>
          <img class="whatscontact" src="whats.svg" alt="whatsapp">
        </a>
      </p>
      
    </div>
    {/each}
  </div>
</div>


<style>
  .value {
    float: right;
    font-size: 18px;
    font-weight: 700;
  }

  .whatscontact{
    height: 
    30px;
  }

  a{
    cursor: pointer;
  }
</style>
