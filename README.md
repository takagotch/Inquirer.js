### Inquirer.js
---
https://github.com/SBoudrias/Inquirer.js

```js
{
  filter() {
    return new Promise();
  },
  
  validate: function (input) {
    var done = this.async();
    
    setTimeout(function() {
     if (typeof input !== 'number') {
       done('You need to provide a number');
       return;
     }
     done(null, true);
    }, 3000);
  }
}

var prompt = inquirer.createPromptModule();
prompt(questions).then();

var inquirer = require('inquirer');
inquirer
  .prompt([
  ])
  .then(answers => {
  });

var prompts = new Rx.Subject();
inquirer.prompt(prompts);

prompts.next({
});
prompts.next({
});
prompts.complete();

inquirer.prompt(prompts).ui.process.subscribe(onEachAnswer, onError, onComplete);

var ui = new inquirer.ui.BottomBar();
outputStream.pipe(ui.log);
ui.log.write('something just happenned.');
ui.log.write('Almost over, standby!');
ui.updateBottomBar('new bottom bar content');
```

```
npm install inquirer

node packages/inquirer/examples/pizza.js
node packages/inquirer/examples/checkbox.js
```

