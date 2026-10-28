
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Inscrição dos jifs IFCE</title>
</head>

<body>
    <header>
        <h1>Inscrição nos jifs</h1>
        Preencha os campos abaixo com suas informações.
    </header>
    <main>
        <form 
            id="inscricao-jifs" action="/inscricoes-jifs" method="post" enctype="multipart/form-data">


            <fieldset>
                <legend>Identificação do atleta</legend><br>

                <label for="nome-atleta">Nome completo (obrigatório)</label>
                <input type="text" id="nome-atleta" name="nome_atleta" required><br><br>

                <label for="email-atleta">E-mail de contato (obrigatório)</label>
                <input type="email" id="email-atleta" name="email_atleta" required>
            </fieldset>


            <fieldset>
                <legend>Participação nos jogos</legend>


                <fieldset>
                    <legend>Turno de preferência</legend>
                    <input type="radio" id="turno-manha" name="turno" value="manha">
                    <label for="turno-manha">Manhã</label>
                    <input type="radio" id="turno-tarde" name="turno" value="tarde">
                    <label for="turno-tarde">Tarde</label>
                    <input type="radio" id="turno-manha" name="turno" value="ambos">
                    <label for="turno-manha">Manhã/tarde</label>
                </fieldset>


                <fieldset>
                    <legend>Modalidades de interesse</legend>
                    <input type="checkbox" id="interesse-futsal" name="modalidades" value="futsal">
                    <label for="interesse-futsal">Futsal</label>
                    <input type="checkbox" id="interesse-volei" name="modalidades" value="voleibol">
                    <label for="interesse-volei">Voleibol</label>
                    <input type="checkbox" id="interesse-volei" name="modalidades" value="Basquete">
                    <label for="interesse-volei">Basquete</label>
                    <input type="checkbox" id="interesse-volei" name="modalidades" value="Natação">
                    <label for="interesse-volei">Natação</label>
                </fieldset>


                <label for="modalidade-principal">Modalidade principal (obrigatória)</label>
                <select id="modalidade-principal" name="modalidade_principal" required>
                    <option value="">Escolha uma modalidade</option>
                    <optgroup label="Coletivas">
                        <option value="futsal">Futsal</option>
                        <option value="voleibol">Voleibol</option>
                         <option value="Basquete">Basquete</option>

                    </optgroup>
                    <optgroup label="Individuais">
                        <option value="atletismo">Atletismo</option>
                        <option value="Dama">Dama</option>
                         <option value="Natação">Natação</option>
                    </optgroup>
                </select>

                <label for="escola">ifce de origem (obrigatória)</label>
                <input type="search" id="escola" name="escola" list="escolas">
                <datalist id="escolas">
                    <option value="IFCE CEDRO"></option>
                    <option value="IFCE IGUATU"></option>
                    <option value="IFCE FORTALEZA"></option>
                    <option value="IFCE JAGUARIBE"></option>
                </datalist>
            </fieldset>

        </form>
    </main>
</body>

</html>
