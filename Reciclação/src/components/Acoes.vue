<template>
  <div class="acoes">
    <section>
      <div class="menu">  
        <h1 class="menu-titulo">Ações</h1>
          <ul>
            <li class="menuAcoes01">Encontros com Escolas >></li>
            <li class="menuAcoes02">Cefé no ponto >></li>
            <li class="menuAcoes03">Palestras temáticas >></li>
            <li class="menuAcoes04">Mutirão de limpeza >></li>
            <li class="menuAcoes05">10 min contra o Aedes Aegypti >></li>
            <li class="menuAcoes06">Coleta seletiva >></li>
          </ul>
      </div>
      <div class="acoes-proxima">
        <p class="acoes-proxima-titulo">Próximas ações</p>
        <ul v-for="evento in eventos_acoes">
          <li>
            <div>
              <div class="descricao-evento">                  
              </div>
            </div>      
          </li>       
        </ul>   
      </div>
    </section> 
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      eventos_acoes: [

      ]
    }
  }
}
</script>

<style scoped>

.acoes {
  background-image: url(../assets/fundo-acoes.jpg);
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;

}

section {
  background: rgba(133, 194, 38, 0.7);
  background-size: 100%;
 
  display: flex;
  flex-direction: row;
}

.menu{
  display: flex;
  flex-direction: column;
  padding: 5%;
  width: 50%;
}

.menu-titulo{  
  color: #fff;
  font-family: 'Roboto Slab';
  font-weight: bold;
  font-size:  3em;
  margin: 0 0 4px 0;
}

ul {
  display: flex;
  justify-content: center;
  align-content: center;
  flex-direction: column;
  margin: 2px;
  padding: 0;
}

li {
  display: flex;
  list-style: none;
  color: #E67816;
  margin: 0;
  padding: 1%;  
  background-color: white;  
  font-family: 'Roboto Slab';
  font-weight: bold;
  font-size: 25px;
}

.menuAcoes01 {
  width: 25vw;
  padding: 15px;
}

.menuAcoes02 {
  width: 16vw;
  padding: 15px;
}
.menuAcoes03 {
  width: 22vw;
  padding: 15px;
}
.menuAcoes04 {
  width: 22vw;
  padding: 15px;
}
.menuAcoes05 {
  width: 32vw;
  padding: 15px;
}
.menuAcoes06 {
  width: 17vw;
  padding: 15px;
}

.acoes-proxima{
  background: #fff;
  width: 36vw;
  height: 95vh;
  margin: 17px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.acoes-proxima-titulo{
  font-family: 'Roboto Slab, Regular';
  font-size: 37px;
  color: #00923F;
}

</style>