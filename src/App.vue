<template>
  <Header></Header>
  <Componente :tabla="t1.tabla"></Componente>
  <Componente :tabla="t2.tabla"></Componente>
</template>

<script>
import Componente from './components/MyComponent.vue'
import Header from './components/Header.vue'

export default {
  name: 'App',
  data() {
    return {
        t1: {
          tabla: {
              title: 'Tabla de datos con Componentes - Hamburguesas',
              headtable: ['Index', 'Imagen', 'Descripcion', 'Precio'],
              productos: 
              [
                  {
                      url: 'hamburguesa.jpg',
                      descripcion: 'Hamburguesa simple',
                      precio: 100
                  },
                  {
                      url: 'hamburguesa.jpg',
                      descripcion: 'Hamburguesa doble',
                      precio: 200
                  },
                  {
                      url: 'hamburguesa.jpg',
                      descripcion: 'Hamburguesa triple',
                      precio: 300
                  }
              ],
              fondo: 'bg-yellow-300'
                }
            },
        t2: {
            tabla: {
                title: 'Tabla de datos con Componentes - Autos',
                headtable: ['Index', 'Imagen', 'Descripcion', 'Precio'],
                productos: [
                    {
                        url: 'audi.jpg',
                        descripcion: 'Audi A4',
                        precio: 58000
                    },
                    {
                        url: 'audi.jpg',
                        descripcion: 'Audi A5',
                        precio: 68000
                    },
                    {
                        url: 'audi.jpg',
                        descripcion: 'Audi A5',
                        precio: 78000
                    }
                ],
                fondo: 'bg-orange-300'
            }
        }
    }
  },
  components: {
    Componente, 
    Header
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
