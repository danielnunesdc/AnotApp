Como resolvi o seguinte erro.

**"Cannot find namespace 'firebase'."**

Solução: entrei no package.json do projeto e defini alguma versão anterior do firebase para ficar acordo com esse projeto.

__Exemplo:__ Procure por **angularfire2** e **firebase** nas dependências, remove o ```^``` e defina uma versão anterior como o modelo abaixo:

```bash
  "dependencies": {
      "angularfire2": "5.0.0-rc.4",
      "firebase": "4.8.0",
  },
``` 
  
Salve o arquivo.

Rode o ```npm install``` e depois o ```ionic serve``` 

Se tudo correr bem, deverá rodar sem mais erros.

O Firebase havia introduzido algumas mudanças que causou ruptura em alguns imports com as quais a AngularFire2 ainda não tinha enfrentado. Até a equipe AngularFire2 resolver, esta será a solução.
