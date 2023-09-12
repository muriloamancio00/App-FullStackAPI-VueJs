<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <!-- Inicio do card de Busca -->
                <card-component titulo="Busca de marcas">
                    <template v-slot:conteudo>
                        <div class="form-row">
                            <div class="col mb-3">

                                <input-container-component titulo="ID" id="InputId" id-help="idHelp"
                                                           texto-ajuda="Opcional. Informe o ID da Marca">
                                    <input type="number" class="form-control" id="inputId" aria-describedby="idHelp"
                                           placeholder="ID">
                                </input-container-component>

                            </div>
                            <div class="col mb-3">

                                <input-container-component titulo="Nome da Marca" id="InputNome" id-help="NomeHelp"
                                                           texto-ajuda="Opcional. Informe o Nome da Marca">
                                    <input type="text" class="form-control" id="inputNome" aria-describedby="idNome"
                                           placeholder="Nome da marca">
                                </input-container-component>
                            </div>
                        </div>
                    </template>
                    <template v-slot:rodape>
                        <button type="submit" class="btn btn-primary btn-sm float-right">Pesquisar</button>
                    </template>
                </card-component>
                <!-- Fim do card de Busca -->

                <!-- Inicio do card de Listagem de Marcas -->
                <card-component titulo="Relação das Marcas">
                    <template v-slot:conteudo>
                        <table-component></table-component>
                    </template>
                    <template v-slot:rodape>
                        <button type="button" class="btn btn-primary btn-sm float-right " data-toggle="modal" data-target="#modalMarca">Adicionar</button>
                    </template>
                </card-component>

                <!-- Fim da Listagem de Marcas -->
            </div>
        </div>
        <!-- Button trigger modal -->
        <modal-component id="modalMarca" titulo="Adicionar Marca"></modal-component>


    </div>
</template>

<script>

import {defineComponent} from "vue";
import Card from "./Card.vue";

export default defineComponent({
    components: {Card}
})
</script>
