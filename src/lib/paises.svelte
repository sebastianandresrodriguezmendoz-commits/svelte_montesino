<script>
    export let pais;
    let p;
    /*[0]=nombre_pais [1]=capital [2]=poblacion  [3]=moneda [4]=continente [5]=bandera]*/
    const paises={
        "colombia":["colombia","bogota","51,52millones","peso colombiano","1.142millones km²","flag_of_colombia.svg"],
        "venezuela":["venezuela","caracas","28,2millones","bolivar","916.445km²","flag_of_venezuela.svg"],
        "ecuador":["ecuador","quito","17,8millones","dolar estadounidense","256.370km²","flag_of_ecuador.svg"],
        "peru":["peru","lima","33,72millones","sol peruano","1.285.215millones km²","800px-flag_of_peru(state).svg.webp"],
        "brazil":["brazil","brasilia","214,3millones","real brasileño","8.51millones km²","flag_of_brazil.svg"],
    }
    p=paises[pais];
</script>
<div class="main">
    <div class="col1">
        <img src=./src/assets/{p[5]} alt="bandera_colombia" width="300" height="150">
    </div>
    <div class="col2">
      <div class="linea"><strong>pais: {p[0]}</strong></div>
      <div class="linea"><strong>capital: {p[1]}</strong></div>
      <div class="linea"><strong>poblacion: {p[2]}</strong></div>
      <div class="linea"><strong>moneda: {p[3]}</strong></div>
      <div class="linea"><strong>extension: {p[4]}</strong></div>
    </div>
</div>
<style>
  .main {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 5px;
    grid-auto-rows: minmax(100px, auto);
    border-radius: 10px;
    border-style: solid;
    border-color: rgb(186, 190, 182);
    border-width: 2px;
    margin: left;
    width: 600px;
    box-shadow: 5px 5px 5px black;
    margin-right: 5px;
    margin-bottom: 10px;
  }
  .col1 {
    grid-column: 1;
    grid-row: 1;
    margin: 5px;
    padding: 5px;
  }
  .col2 {
    grid-column: 2;
    grid-row: 1;
    margin: 5px;
    padding: 5px;
    border-color: black;
    width: max-content;
  }
  strong {
    color: blue;
    font-weight: bolder;
  }
  .linea {
    font-size: 20px;
    margin-bottom: 18px;
  }
</style>