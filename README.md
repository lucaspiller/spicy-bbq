# Spicy BBQ

Spicy BBQ is a simple script which will combine a directory of assets into a single Javascript file. It encodes the assets using Data URI encoding which is supported by all modern browsers. It is aimed to be used in rich client Javascript applications, specifically with JST templates.

## Requirements

Spicy BBQ is written in shell script, and only uses common tools found on nix systems. If you are on OS X or Linux it should just work. If it doesn't, let me know why!

## Usage

Just point it to your assets directory:

    spicy_bbq public/images > build/javascripts/sb.js

Then in your Javascript, just pass the filename to SB, for example in a JST template:

    <img src="<%= SB['message_reply.png'] %>" alt="Reply" />

## Contributing

* Fork the project.
* Make your feature addition or bug fix.
* Send me a pull request. Bonus points for topic branches.
* Add tests for what you are building, and make sure you don't break any existing tests.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/InteractiveResource" property="dct:title" rel="dct:type">spicy-bbq</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/lucaspiller/spicy-bbq" property="cc:attributionName" rel="cc:attributionURL">Luca Spiller</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/">Creative Commons Attribution-ShareAlike 3.0 Unported License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/lucaspiller/spicy-bbq" rel="dct:source">github.com</a>.<br />Permissions beyond the scope of this license may be available at <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/lucaspiller/spicy-bbq" rel="cc:morePermissions">https://github.com/lucaspiller/spicy-bbq</a>.
