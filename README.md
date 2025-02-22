# amigo-secreto
const fs = require('fs');

const tituloProjeto = 'Projeto Amigo Secreto;
const descricaoProjeto = 'Este projeto tem como objetivo adicionaramigos e escolher aleatóriamente um amigo.';

const conteudoReadme = `# ${tituloProjeto}

${descricaoProjeto}
`;

fs.writeFile('README.md', conteudoReadme, (err) => {
  if (err) {
    console.error('Erro ao criar o arquivo README:', err);
  } else {
    console.log('Arquivo README criado com sucesso!');
  }
});
