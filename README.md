# progWeb

<html>

<head>
  <meta charset="utf-8"/>
  <title="Instituto de Computação">
</head>

<body>
  <h2>Formulário de Contato</h2>
  <h5>Por favor, preencha o formulário abaixo e clique no botão Enviar Mensagem.
    Agradecemos por seu contato.</h5>

  <fieldset>
    <legend>Dados Básicos</legend>

    <label for="nome">Nome:</label>
    <input type="text" name="nome" id="nome"/><br>

    <label for="email">E-mail </label>
    <input type="email" name="email" id="email" required
     placeholder="seunome@dominio.com.br" ><br>

     <label for="Website">Website:</label>
     <input type="text" name="nome" value="http://" id="nome"/><br>
  </fieldset>

  <fieldset>
    <legend>Seu curso no Instituto de Computação</legend>
    <input type="radio" name="curso" value="cc" id="cc">
    <label for="cc">Ciência da Computação</label><br>

    <input type="radio" name="curso" value="si" id="si">
    <label for="si">Sistemas de Informação</label><br>

    <input type="radio" name="curso" value="ec" id="ec">
    <label for="ec">Engenharia da Computação</label><br>
  </fieldset>

  <fieldset>
    <legend>Assinale as linguagens já usadas por você:</legend>
    <label for="java">Java</label>
      <input type="checkbox" name="ling" id="java" value="java">
    <label for="c">C</label>
      <input type="checkbox" name="ling" id="c" value="c">
    <label for="cpp">C++</label>
      <input type="checkbox" name="ling" id="cpp" value="cpp">
    <label for="perl">Perl</label>
      <input type="checkbox" name="ling" id="perl" value="perl">
    <label for="python">Python</label>
      <input type="checkbox" name="ling" id="python" value="python">
    <label for="js">Javascript</label>
      <input type="checkbox" name="ling" id="js" value="js">
  </fieldset>


  <fieldset>
    <legend>Dados Complementares</legend>
    <label for="cor">Cor favorita</label>
    <input type="color" name="cor" id="cor"><br>

    <label for="nascimento">Data de Nascimento</label>
     <input type="date" name="nascimento" id="nascimento"><br>

     <label for="ano">Ano de Entrada em seu Curso do IComp</label>
      <input type="number" name="ano" min="2000" max="2017"
         step="1" value="2000" id="ano"><br>

    <label for="nota">Nota para este site</label>
    <input type="range" name="nota" min="0" max="10"
    step="1" value="0" id="nota">

  </fieldset>

  <fieldset>
    <legend>Área de Atuação</legend>
   <select name="area" id="area">
     <option value="1">Banco de Dados</option>
     <option value="2">Educação a Distância</option>
     <option value="3">Engenharia de Software</option>
     <option value="4">Otimização</option>
     <option value="5">Programação para a Web</option>
     <option value="6">Recuperação de Informação</option>
     <option value="7">Redes de Computadores</option>
   </select>
 </fieldset>

 <fieldset>
 <legend>Submeta seu currículo vitae</legend>
 <input type="file" name="curriculo">
</fieldset>

 <fieldset>
 <legend>Digite sua mensagem</legend>
 <textarea name="mensagem" rows="4" cols="50" onfocus="this.value='';">
  Este é o valor padrão!
 </textarea>
 </fieldset><br>

 <form id="contact" method="GET" action="processa.php">
  <input type="reset" value="Resetar Dados" />
  <input type="submit" name="submit" value="Enviar Mensagem" />
 </form>

</body>

</html>
