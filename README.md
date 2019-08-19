### generator-jhipster
---
https://github.com/jhipster/generator-jhipster

```js
// test/app.spec.js

describe('JHipster generator', () => {
  context('Default configuration with', () => {
    describe('AngularX', () => {
      before(done => {
        helpers
          .run(path.join(__dirname, '../generators/app'))
          .withOptions({ 'from-cli': true, skipInstall: true, skipChecks: true, jhiPrefix: 'test'})
          .withPrompts({
            baseName: 'jhipster',
            clientFramework: 'angularX',
            packageName: 'com.mycompany.myapp',
          })
          .on('end', done);
      });
      
      it('creates expected default files for angularX', () => {
        assert.file(expectedFiles.common);
        assert.file(expectedFiles.server);
        assert.file(expectedFiles.userManagementServer);
      });
      it('contains clientFramework with angularX value', () => {
        assert.fileContent('.yo-rc.json', /"clientFramework": "angularX"/);
      });
    });
    
    describe('React', () => {
      before(done => {
        .run(path.join(__dirname, '../generateors/app'))
        .withOptions({
          'from-cli': true,
          skipInstall: true,
          skipChecks: true,
          jhiPrefix: 'test',
          experimental: true
        })
        .withPrompts({
          baseName: 'jhipster',
          clientFramework: 'react',
        })
      })
    })
  })
})


```

```
```

```
```
