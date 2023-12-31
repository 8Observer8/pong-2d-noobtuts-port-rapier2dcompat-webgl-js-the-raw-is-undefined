[Issue](https://github.com/dimforge/rapier.js/issues/240)

The problem is described in this topic: https://discord.com/channels/507548572338880513/1128683241436631140

Sandboxes:

- PlayCode: https://playcode.io/1531297
- Plunker: https://plnkr.co/edit/ee9vdQPHTW1f9QSO?preview

Install these packages globally with the command:

> npm i -g http-server rollup uglify-js

Run http-server in the project directory:

> http-server -c-1

Note. The `-c-1` key allows you to disable caching.

Start development mode with the following command:

> npm run dev

Note. Rollup will automatically keep track of saving changes to files and build a new index.js file ready for debugging. You can debug your project step by step in the browser by setting breakpoints.

Create a compressed file ready for publishing. Stop development mode, for example, with this command Ctrl + C in CMD, if it was launched before and enter the command:

> npm run release

Note. After this command, Rollup will create a compressed index.js file. Compression is done using the uglify-js package.
