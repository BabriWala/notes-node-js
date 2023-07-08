Modules are the collection of JavaScript codes in a separate logical file that can be used in external applications on the basis of their related functionality.

Enable Use Module by .mjs extention or write type: module
https://blog.logrocket.com/commonjs-vs-es-modules-node-js/

For browser support, all major browsers support the ES module syntax and you can use import/export in frameworks like React and Vue.js. These frameworks uses a transpiler like Babel to compile the import/export syntax down to require(), which older Node.js versions natively support.

Named exports
module.exports.name = "Alex"

Default exports
export default function sayName() {console.log('My name is Mat')}
module.exports = {sayName, sayAge};


The signature of the wrapper function is shown below:
(function(exports, require, module, __filename, __dirname) {
// Module code actually lives in here
});

important: https://reflectoring.io/nodejs-modules-imports/

https://blog.logrocket.com/es-modules-in-node-today/#commonjsmodulesystem