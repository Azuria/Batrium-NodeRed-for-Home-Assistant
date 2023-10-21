# Batrium-NodeRed-for-Home-Assistant
My Node-Red flow for Batrium in Home Assistant.

Requires Home Assistant Node-Red configuration to include: 
npm_packages:
  - binary-parser


Also /config/node-red/settings.js should have the functionsGlobalContext section filled out with:
  
  functionGlobalContext: {
    // os:require('os'),
    // jfive:require("johnny-five"),
    // j5board:require("johnny-five").Board({repl:false})
    binary_parser:require('binary-parser').Parser,
  },
