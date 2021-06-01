<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="{{asset('css/painel.css')}}" type="text/css">
    <link rel="stylesheet" href="{{asset('css/bootstrap.css')}}" type="text/css">
    <link rel="stylesheet" href="{{asset('css/bootstrap.min.css')}}" type="text/css">
    <script src="{{asset('js/jquery-3.5.1.min.js')}}"></script>
    <script src="{{asset('js/bootstrap.min.js')}}"></script>
    <meta name="csrf-token" content="{{ csrf_token() }}">
    <title>Painel</title>
</head>
<body>
   
    <nav class="navbar navbar-expand-lg navbar navbar-light" style="background-color: #3a6475;">
        <div class="container-fluid">
            <a class="navbar-brand" href="#" style="color: white;">X-Cópias</a>
            
            <button style="background-color: white;" class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse"  id="navbarSupportedContent">
            <div>
                <ul class="navbar-nav mr-auto">
                    <li class="nav-item">
                        <a class="nav-link" style="color: white;">inicio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="/perfil" style="color: white;">perfil</a>
                    </li>
                </ul>
            </div>
            <div class="buttonexit">
                <a href="/logout"><button  class="btn btn-outline-light" type="submit">sair</button></a>
            </div>
            </div>
        </div>
    </nav>    
    <div class="container">
        <div class="row">
            <div>
                <button onclick="cadastrar()" type="button" class="btn btn-secondary" style="background-color: #3a6475;">novo professor</button>
                <button onclick="getrelatorio()"type="button" class="btn btn-secondary" style="background-color: #3a6475;">ver relatório</button>
            </div>
        </div>
        <div class="row" style="margin-top: 20px;">
            @foreach($usuarios as $user)
            <div class="col">
                <div class="userinfos">
                    <span style="font-family: sans-serif; font-size: 18px;">Professor</span>
                    <span style="font-family: sans-serif; font-size: 16px;">{{$user->name}}</span>
                </div>
                <div class="copiasinfo">
                    <span >Cópias mensal: <span style="color: #0b6a8d;">{{$user->copiasmes}}</span></span>
                    <span>Cópias restante: <span style="color: #0b6a8d;">{{$user->copiasrestante}}</span></span>
                </div>
                <div class="btn-group" role="group" aria-label="Basic outlined example">
                    <button type="button" onclick="retirarcopias({{$user->id}})"  class="btn btn-outline-dark" >retirar</button>
                    <button type="button" onclick="retornarcopias({{$user->id}})" class="btn btn-outline-dark">retornar</button>
                    <button type="button" onclick="renovarcopias({{$user->id}})"  class="btn btn-outline-dark">renovar</button>
                </div>
            </div>
            @endforeach
        </div>
    </div>

    
    <!-- Modal -->
    <div class="modal fade" id="exampleModalcaduser" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog" role="document">
            <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title" id="exampleModalLabel">Cadastro de professores</h5>
                <button id="modalClose" type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
                </button>
            </div>
            <div class="modal-body">
                <form>
                    <div class="form-group">
                        <label for="recipient-name" class="col-form-label">nome</label>
                        <input type="text" class="form-control" name="nomecad" id="recipient-name" placeholder="nome do novo professor...">
                    </div>
                    <div class="form-group">
                        <label for="recipient-username" class="col-form-label">usuário:</label>
                        <input type="text" class="form-control" name="usernamecad" id="recipient-username" placeholder="usuário...">
                    </div>
                    <div class="form-group">
                        <label for="recipient-password" class="col-form-label">senha:</label>
                        <input type="password" class="form-control" name="passcad" id="recipient-password" placeholder="senha...">
                    </div>
                </form>
                <div style="display: flex; justify-content: center;">
                    <span id="msgcdprof" style="display: none;"></span>
                </div>
            </div>
            <div class="modal-footer">
                <button type="button" onclick="sendcduser()" class="btn btn-secondary" style="background-color: #3a6475;">cadastrar</button>
            </div>
            </div>
        </div>
    </div>

    <div class="modal fade" id="exampleModalLong" tabindex="-1" role="dialog" aria-labelledby="exampleModalLongTitle" aria-hidden="true">
        <div class="modal-dialog" role="document">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="exampleModalLongTitle">Relatório</h5>
                    <button id="modalCloserela" type="button" class="close" data-dismiss="modal" aria-label="Close">
                    <span aria-hidden="true">&times;</span>
                    </button>
                </div>
                <div class="modal-body">
                    <div class="text-center" style="display:none">
                        <div class="spinner-border" role="status">
                            <span class="visually-hidden">Loading...</span>
                        </div>
                    </div>
                    <div class="container" style="margin-top: 5%; display:block;">
                        @foreach($registro as $data)
                        <div class="row">
                            <span style="font-family: sans-serif;">{{date('d/m/Y -- H:i:s', strtotime($data->created_at))}}</span>
                            <div class="row" style="margin-left: 5%;">
                                <span style="font-family: sans-serif;">Ação - <span style="color: #0b6a8d;">{{$data->action}}</span></span>
                                <span style="font-family: sans-serif;">Usuário - <span style="color: #0b6a8d;">{{$data->user}}</span></span>
                                <span style="font-family: sans-serif;">Quantidade - <span style="color: #0b6a8d;">{{$data->quant}}</span></span>
                            </div>
                        </div>
                        <hr>
                        @endforeach
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="modal fade" id="exampleModalreti" tabindex="-1" role="dialog" aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered" role="document">
            <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title" id="exampleModalLongTitle">Retirar cópias</h5>
                <button id="modalClosereti" type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
                </button>
            </div>
            <div class="modal-body">
                <form>
                    <input type="hidden" id="rtid" name="idrt" value="">
                    <div class="form-group">
                        <label for="recipient-reti" class="col-form-label">quantidade</label>
                        <input type="number" class="form-control" name="quantrt" id="recipient-reti">
                    </div>
                </form>
                <div style="display: flex; justify-content: center;">
                    <span id="msgreti" style="color: red;"></span>
                </div>
            </div>
            <div class="modal-footer">
                <button type="button" onclick="sendretirar()" class="btn btn-secondary" style="background-color: #3a6475;">salvar</button>
            </div>
            </div>
        </div>
    </div>

    <div class="modal fade" id="exampleModalreto" tabindex="-1" role="dialog" aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered" role="document">
            <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title" id="exampleModalLongTitle">Retornar cópias</h5>
                <button id="modalClosereto" type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
                </button>
            </div>
            <div class="modal-body">
                <input type="hidden" id="rtoid" name="idrto" value="">
                <form>
                    <div class="form-group">
                        <label for="recipient-reto" class="col-form-label">quantidade</label>
                        <input type="number" class="form-control" name="quantrto" id="recipient-reto">
                    </div>
                </form>
                <div style="display: flex; justify-content: center;">
                    <span id="msgreto" style="color: red;"></span>
                </div>
            </div>
            <div class="modal-footer">
                <button type="button" onclick="sendretornar()" class="btn btn-secondary" style="background-color: #3a6475;">salvar</button>
            </div>
            </div>
        </div>
    </div>

    <div class="modal fade" id="exampleModalreno" tabindex="-1" role="dialog" aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered" role="document">
            <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title" id="exampleModalLongTitle">Renovar cópias</h5>
                <button id="modalClosereno" type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
                </button>
            </div>
            <div class="modal-body">
            <input type="hidden" id="rnid" name="idrn" value="">
                <form>
                    <div class="form-group">
                        <label for="recipient-reno" class="col-form-label">quantidade</label>
                        <input type="number" class="form-control" name="quantrn" id="recipient-reno">
                    </div>
                </form>
                <div style="display: flex; justify-content: center;">
                    <span id="msgreno" style="color: red;"></span>
                </div>
            </div>
            <div class="modal-footer">
                <button type="button" onclick="sendrenovar()" class="btn btn-secondary" style="background-color: #3a6475;">salvar</button>
            </div>
            </div>
        </div>
    </div>
    <script>
    
        function cadastrar(){
            $('#exampleModalcaduser').modal('show')
            $(function () {
                $('#modalClose').on('click', function () {
                    $('#exampleModalcaduser').modal('hide');
                })
            })
        }
        function getrelatorio(){
        
        $('#exampleModalLong').modal('show')
            $(function () {
                $('#modalCloserela').on('click', function () {
                    $('#exampleModalLong').modal('hide');
                })
            })
        }

        function retirarcopias(id){
            document.getElementById('rtid').value = id;
            $('#exampleModalreti').modal('show')
            $(function () {
                $('#modalClosereti').on('click', function () {
                    $('#exampleModalreti').modal('hide');
                })
            })
        }

        function retornarcopias(id){
            document.getElementById('rtoid').value = id;
            $('#exampleModalreto').modal('show')
            $(function () {
                $('#modalClosereto').on('click', function () {
                    $('#exampleModalreto').modal('hide');
                })
            })
        }
        function renovarcopias(id){
            document.getElementById('rnid').value = id;
            $('#exampleModalreno').modal('show')
            $(function () {
                $('#modalClosereno').on('click', function () {
                    $('#exampleModalreno').modal('hide');
                })
            })
        }
    

        function sendcduser(){
            $.ajaxSetup({
                headers: {
                    'X-CSRF-TOKEN': $('meta[name="csrf-token"]').attr('content')
                }
            });
            data = {
                nome: $("input[name=nomecad]").val(),
                username: $("input[name=usernamecad]").val(),
                pass: $("input[name=passcad]").val()
            },
            $.ajax({
                type: "POST",
                url: "{{route('cduser')}}",
                data: data,
                success: function(response) {
                    if(response["msgnotok"]){
                        document.getElementById("msgcdprof").style.color = "red";
                        document.getElementById("msgcdprof").style.display = 'block';
                        document.getElementById("msgcdprof").innerText = response["msgnotok"];
                    }
                    else{
                        document.getElementById("msgcdprof").style.color = "green";
                        document.getElementById("msgcdprof").style.display = 'block';
                        document.getElementById("msgcdprof").innerText = "professor cadastrado";
                    }
                },
                error: (e) => {
                    alert('Erro no processo');
                },
            });
        }



        function sendretirar(){
            $.ajaxSetup({
                headers: {
                    'X-CSRF-TOKEN': $('meta[name="csrf-token"]').attr('content')
                }
            });
            data = {
                id: $("input[name=idrt]").val(),
                quantidade: $("input[name=quantrt]").val()
            },
            $.ajax({
                type: "POST",
                url: "{{route('rtcopias')}}",
                data: data,
                success: function(response) {
                    if(response['msgnotok']){
                        document.getElementById("msgreti").innerText = response["msgnotok"];
                    }else{
                        window.location.href = "{{route('padm')}}"
                    }
                },
                error: (e) => {
                    alert('Erro no processo');
                },
            });
        }

        function sendretornar(){
            $.ajaxSetup({
                headers: {
                    'X-CSRF-TOKEN': $('meta[name="csrf-token"]').attr('content')
                }
            });
            data = {
                id: $("input[name=idrto]").val(),
                quantidade: $("input[name=quantrto]").val()
            },
            $.ajax({
                type: "POST",
                url: "{{route('rtocopias')}}",
                data: data,
                success: function(response) {
                    if(response['msgnotok']){
                        document.getElementById("msgreto").innerText = response["msgnotok"];
                    }else{
                        window.location.href = "{{route('padm')}}"
                    }
                },
                error: (e) => {
                    alert('Erro no processo');
                },
            });
        }

        function sendrenovar(){
            $.ajaxSetup({
                headers: {
                    'X-CSRF-TOKEN': $('meta[name="csrf-token"]').attr('content')
                }
            });
            data = {
                id: $("input[name=idrn]").val(),
                quantidade: $("input[name=quantrn]").val()
            },
            $.ajax({
                type: "POST",
                url: "{{route('rncopias')}}",
                data: data,
                success: function(response) {
                    if(response['msgnotok']){
                        document.getElementById("msgreno").innerText = response["msgnotok"];
                    }else{
                        window.location.href = "{{route('padm')}}"
                    }
                },
                error: (e) => {
                    alert('Erro no processo');
                },
            });
        }
    </script>
</body>
</html>