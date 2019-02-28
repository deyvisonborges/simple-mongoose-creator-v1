# :trollface: Simple Mongoose Creator
Com este módulo você vai economizar linhas de código durante a criação de
esquemas com o mongoose, simples assim.
```
Observação:
"Este é apenas um beta e vai ter muito mais melhorias, devido à inumeras funcionalidades que o 
módulo, por enquanto, não nos permite desfrutar."
```
## Sem o módulo
```  
    const mongoose = require('mongoose');
    const schema = mongoose.Schema;
    const model = new schema({object});

    module.exports = mongoose.model('collection_name', model);
```  

## Com o módulo
```  
    const schema = require('../mongoose-creator')
    module.exports = schema('collection_name', {object})
```