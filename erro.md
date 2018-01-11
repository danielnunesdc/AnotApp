Como resolvi o seguinte erro.

**"Cannot find namespace 'firebase'."**

De acodo com o que pesquisei, a partir da versão 4.8.1 do firebase ouve algumas refatorações nos imports da biblioeca.

Solução 1: Renomear tudo que pareceu errado.

Solução 2: entrei no package.json do projeto e defini alguma versão anterior do firebase para ficar acordo com esse projeto.

__Exemplo:__ Procure por **angularfire2** e **firebase** nas dependências e defina as seguintes versões:

```bash
  "dependencies": {
      "angularfire2": "5.0.0-rc.4",
      "firebase": "4.8.0",
  },
``` 
  
Salve o arquivo.

Rode o ```npm install``` e depois o ```ionic serve``` 

Se tudo correr bem, deverá rodar sem mais erros.
