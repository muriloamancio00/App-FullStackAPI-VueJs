<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <!-- Inicio do card de Busca -->
                <div class="card mb-3">
                    <div class="card-header">Busca de Marcas</div>

                    <div class="card-body">
                        <div class="form-row">
                            <div class="col mb-3">

                                <input-container-component
                                    titulo="ID"
                                    id="InputId"
                                    id-help="idHelp"
                                    texto-ajuda="Opcional. Informe o ID da Marca">

                                    <input type="number" class="form-control" id="inputId" aria-describedby="idHelp"
                                           placeholder="ID">
                                </input-container-component>

                            </div>
                            <div class="col mb-3">

                                <input-container-component
                                    titulo="Nome da Marca"
                                    id="InputNome"
                                    id-help="NomeHelp"
                                    texto-ajuda="Opcional. Informe o Nome da Marca">

                                    <input type="text" class="form-control" id="inputNome" aria-describedby="idNome"
                                           placeholder="Nome da marca">
                                </input-container-component>
                            </div>
                        </div>
                    </div>
                    <div class="card-footer">
                        <button type="submit" class="btn btn-primary btn-sm float-right">Pesquisar</button>
                    </div>
                </div>
                <!-- Fim do card de Busca -->

                <!-- Inicio do card de Listagem de Marcas -->

                <div class="card">
                    <div class="card-header">Relação das Marcas</div>

                    <div class="card-body">
                        <table-component></table-component>
                    </div>
                    <div class="card-footer">
                        <button type="button" class="btn btn-primary btn-sm float-right">Adicionar</button>
                    </div>
                </div>

                <!-- Fim da Listagem de Marcas -->
            </div>
        </div>
    </div>
</template>

<script>

</script>
