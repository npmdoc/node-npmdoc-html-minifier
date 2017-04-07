# api documentation for  [html-minifier (v3.4.2)](http://kangax.github.io/html-minifier/)  [![npm package](https://img.shields.io/npm/v/npmdoc-html-minifier.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-html-minifier) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-html-minifier.svg)](https://travis-ci.org/npmdoc/node-npmdoc-html-minifier)
#### Highly configurable, well-tested, JavaScript-based HTML minifier.

[![NPM](https://nodei.co/npm/html-minifier.png?downloads=true)](https://www.npmjs.com/package/html-minifier)

[![apidoc](https://npmdoc.github.io/node-npmdoc-html-minifier/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-html-minifier%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-html-minifier/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-html-minifier/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-html-minifier/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Juriy \"kangax\" Zaytsev"
    },
    "benchmarkDependencies": {
        "brotli": "1.3.x",
        "chalk": "1.1.x",
        "cli-table": "0.3.x",
        "lzma": "2.3.x",
        "minimize": "2.1.x",
        "progress": "1.1.x"
    },
    "bin": {
        "html-minifier": "./cli.js"
    },
    "bugs": {
        "url": "https://github.com/kangax/html-minifier/issues"
    },
    "contributors": [
        {
            "name": "Gilmore Davidson",
            "url": "https://github.com/gilmoreorless"
        },
        {
            "name": "Hugo Wetterberg",
            "email": "hugo@wetterberg.nu"
        },
        {
            "name": "Zoltan Frombach",
            "email": "tssajo@gmail.com"
        }
    ],
    "dependencies": {
        "camel-case": "3.0.x",
        "clean-css": "4.0.x",
        "commander": "2.9.x",
        "he": "1.1.x",
        "ncname": "1.0.x",
        "param-case": "2.1.x",
        "relateurl": "0.2.x",
        "uglify-js": "2.8.x"
    },
    "description": "Highly configurable, well-tested, JavaScript-based HTML minifier.",
    "devDependencies": {
        "grunt": "1.0.x",
        "grunt-browserify": "5.0.x",
        "grunt-contrib-uglify": "2.2.x",
        "gruntify-eslint": "3.1.x",
        "phantomjs-prebuilt": "2.1.x",
        "qunitjs": "2.x"
    },
    "directories": {},
    "dist": {
        "shasum": "31896baaf735c1d95f7a0b7291f9dc36c0720752",
        "tarball": "https://registry.npmjs.org/html-minifier/-/html-minifier-3.4.2.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "files": [
        "src/*.js",
        "cli.js",
        "sample-cli-config-file.conf"
    ],
    "gitHead": "d8c8680a98212077b637f6289625dcac22a32c16",
    "homepage": "http://kangax.github.io/html-minifier/",
    "keywords": [
        "cli",
        "compress",
        "compressor",
        "css",
        "html",
        "htmlmin",
        "javascript",
        "min",
        "minification",
        "minifier",
        "minify",
        "optimize",
        "optimizer",
        "pack",
        "packer",
        "parse",
        "parser",
        "uglifier",
        "uglify"
    ],
    "license": "MIT",
    "main": "src/htmlminifier.js",
    "maintainers": [
        {
            "name": "alexlamsl",
            "email": "alex+npm@starthq.com"
        },
        {
            "name": "kangax",
            "email": "kangax@gmail.com"
        }
    ],
    "name": "html-minifier",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/kangax/html-minifier.git"
    },
    "scripts": {
        "dist": "grunt dist",
        "test": "grunt test"
    },
    "version": "3.4.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module html-minifier](#apidoc.module.html-minifier)
1.  [function <span class="apidocSignatureSpan">html-minifier.</span>minify (value, options)](#apidoc.element.html-minifier.minify)
1.  [function <span class="apidocSignatureSpan">html-minifier.</span>tokenchain ()](#apidoc.element.html-minifier.tokenchain)
1.  object <span class="apidocSignatureSpan">html-minifier.</span>htmlparser
1.  object <span class="apidocSignatureSpan">html-minifier.</span>tokenchain.prototype
1.  object <span class="apidocSignatureSpan">html-minifier.</span>utils

#### [module html-minifier.htmlparser](#apidoc.module.html-minifier.htmlparser)
1.  [function <span class="apidocSignatureSpan">html-minifier.htmlparser.</span>HTMLParser (html, handler)](#apidoc.element.html-minifier.htmlparser.HTMLParser)
1.  [function <span class="apidocSignatureSpan">html-minifier.htmlparser.</span>HTMLtoDOM (html, doc)](#apidoc.element.html-minifier.htmlparser.HTMLtoDOM)
1.  [function <span class="apidocSignatureSpan">html-minifier.htmlparser.</span>HTMLtoXML (html)](#apidoc.element.html-minifier.htmlparser.HTMLtoXML)

#### [module html-minifier.tokenchain](#apidoc.module.html-minifier.tokenchain)
1.  [function <span class="apidocSignatureSpan">html-minifier.</span>tokenchain ()](#apidoc.element.html-minifier.tokenchain.tokenchain)

#### [module html-minifier.tokenchain.prototype](#apidoc.module.html-minifier.tokenchain.prototype)
1.  [function <span class="apidocSignatureSpan">html-minifier.tokenchain.prototype.</span>add (tokens)](#apidoc.element.html-minifier.tokenchain.prototype.add)
1.  [function <span class="apidocSignatureSpan">html-minifier.tokenchain.prototype.</span>createSorter ()](#apidoc.element.html-minifier.tokenchain.prototype.createSorter)

#### [module html-minifier.utils](#apidoc.module.html-minifier.utils)
1.  [function <span class="apidocSignatureSpan">html-minifier.utils.</span>createMap (values, ignoreCase)](#apidoc.element.html-minifier.utils.createMap)
1.  [function <span class="apidocSignatureSpan">html-minifier.utils.</span>createMapFromString (values, ignoreCase)](#apidoc.element.html-minifier.utils.createMapFromString)



# <a name="apidoc.module.html-minifier"></a>[module html-minifier](#apidoc.module.html-minifier)

#### <a name="apidoc.element.html-minifier.minify"></a>[function <span class="apidocSignatureSpan">html-minifier.</span>minify (value, options)](#apidoc.element.html-minifier.minify)
- description and source-code
```javascript
minify = function (value, options) {
  return minify(value, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html-minifier.tokenchain"></a>[function <span class="apidocSignatureSpan">html-minifier.</span>tokenchain ()](#apidoc.element.html-minifier.tokenchain)
- description and source-code
```javascript
function TokenChain() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html-minifier.htmlparser"></a>[module html-minifier.htmlparser](#apidoc.module.html-minifier.htmlparser)

#### <a name="apidoc.element.html-minifier.htmlparser.HTMLParser"></a>[function <span class="apidocSignatureSpan">html-minifier.htmlparser.</span>HTMLParser (html, handler)](#apidoc.element.html-minifier.htmlparser.HTMLParser)
- description and source-code
```javascript
function HTMLParser(html, handler) {
  var stack = [], lastTag;
  var attribute = attrForHandler(handler);
  var last, prevTag, nextTag;
  while (html) {
    last = html;
    // Make sure we're not in a script or style element
    if (!lastTag || !special(lastTag)) {
      var textEnd = html.indexOf('<');
      if (textEnd === 0) {
        // Comment:
        if (/^<!--/.test(html)) {
          var commentEnd = html.indexOf('-->');

          if (commentEnd >= 0) {
            if (handler.comment) {
              handler.comment(html.substring(4, commentEnd));
            }
            html = html.substring(commentEnd + 3);
            prevTag = '';
            continue;
          }
        }

        // http://en.wikipedia.org/wiki/Conditional_comment#Downlevel-revealed_conditional_comment
        if (/^<!\[/.test(html)) {
          var conditionalEnd = html.indexOf(']>');

          if (conditionalEnd >= 0) {
            if (handler.comment) {
              handler.comment(html.substring(2, conditionalEnd + 1), true /* non-standard */);
            }
            html = html.substring(conditionalEnd + 2);
            prevTag = '';
            continue;
          }
        }

        // Doctype:
        var doctypeMatch = html.match(doctype);
        if (doctypeMatch) {
          if (handler.doctype) {
            handler.doctype(doctypeMatch[0]);
          }
          html = html.substring(doctypeMatch[0].length);
          prevTag = '';
          continue;
        }

        // End tag:
        var endTagMatch = html.match(endTag);
        if (endTagMatch) {
          html = html.substring(endTagMatch[0].length);
          endTagMatch[0].replace(endTag, parseEndTag);
          prevTag = '/' + endTagMatch[1].toLowerCase();
          continue;
        }

        // Start tag:
        var startTagMatch = parseStartTag(html);
        if (startTagMatch) {
          html = startTagMatch.rest;
          handleStartTag(startTagMatch);
          prevTag = startTagMatch.tagName.toLowerCase();
          continue;
        }
      }

      var text;
      if (textEnd >= 0) {
        text = html.substring(0, textEnd);
        html = html.substring(textEnd);
      }
      else {
        text = html;
        html = '';
      }

      // next tag
      var nextTagMatch = parseStartTag(html);
      if (nextTagMatch) {
        nextTag = nextTagMatch.tagName;
      }
      else {
        nextTagMatch = html.match(endTag);
        if (nextTagMatch) {
          nextTag = '/' + nextTagMatch[1];
        }
        else {
          nextTag = '';
        }
      }

      if (handler.chars) {
        handler.chars(text, prevTag, nextTag);
      }
      prevTag = '';

    }
    else {
      var stackedTag = lastTag.toLowerCase();
      var reStackedTag = reCache[stackedTag] || (reCache[stackedTag] = new RegExp('([\\s\\S]*?)</' + stackedTag + '[^>]*>', 'i'));

      html = html.replace(reStackedTag, function(all, text) {
        if (stackedTag !== 'script' && stackedTag !== 'style' && stackedTag !== 'noscript') {
          text = text
            .replace(/<!--([\s\S]*?)-->/g, '$1')
            .replace(/<!\[CDATA\[([\s\S]*?)]]>/g, '$1');
        }

        if (handler.chars) {
          handler.chars(text);
        }

        return '';
      });

      parseEndTag('</' + stackedTag + '>', stackedTag);
    }

    if (html === last) {
      throw new Error('Parse Error: ' + html);
    }
  }

  if (!handler.partialMarkup) {
    // Clean up any remaining tags
    parseEndTag();
  }

  function parseStartTag(input) {
    var start = input.match(startTagOpen);
    if (start) {
      var match = {
        tagName: start[1],
        attrs: []
      };
      input = input.slice(start[0].length);
      var end, attr;
      while (!(end = input.match(startTagClose)) && (attr = input.match(attribute))) {
        input = input.slice(attr[0].length);
        match.attrs.push(attr);
      }
      if (end) {
        match.unarySlash = end[1];
        match.rest = input.slice(end[0].length);
        return match;
      }
    }
  }

  function handleStartTag(match ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html-minifier.htmlparser.HTMLtoDOM"></a>[function <span class="apidocSignatureSpan">html-minifier.htmlparser.</span>HTMLtoDOM (html, doc)](#apidoc.element.html-minifier.htmlparser.HTMLtoDOM)
- description and source-code
```javascript
HTMLtoDOM = function (html, doc) {
  // There can be only one of these elements
  var one = {
    html: true,
    head: true,
    body: true,
    title: true
  };

  // Enforce a structure for the document
  var structure = {
    link: 'head',
    base: 'head'
  };

  if (doc) {
    doc = doc.ownerDocument || doc.getOwnerDocument && doc.getOwnerDocument() || doc;
  }
  else if (typeof DOMDocument !== 'undefined') {
    doc = new DOMDocument();
  }
  else if (typeof document !== 'undefined' && document.implementation && document.implementation.createDocument) {
    doc = document.implementation.createDocument('', '', null);
  }
  else if (typeof ActiveX !== 'undefined') {
    doc = new ActiveXObject('Msxml.DOMDocument');
  }

  var elems = [],
      documentElement = doc.documentElement ||
        doc.getDocumentElement && doc.getDocumentElement();

  // If we're dealing with an empty document then we
  // need to pre-populate it with the HTML document structure
  if (!documentElement && doc.createElement) {
    (function() {
      var html = doc.createElement('html');
      var head = doc.createElement('head');
      head.appendChild(doc.createElement('title'));
      html.appendChild(head);
      html.appendChild(doc.createElement('body'));
      doc.appendChild(html);
    })();
  }

  // Find all the unique elements
  if (doc.getElementsByTagName) {
    for (var i in one) {
      one[i] = doc.getElementsByTagName(i)[0];
    }
  }

  // If we're working with a document, inject contents into
  // the body element
  var curParentNode = one.body;

  new HTMLParser(html, {
    start: function(tagName, attrs, unary) {
      // If it's a pre-built element, then we can ignore
      // its construction
      if (one[tagName]) {
        curParentNode = one[tagName];
        return;
      }

      var elem = doc.createElement(tagName);

      for (var attr in attrs) {
        elem.setAttribute(attrs[attr].name, attrs[attr].value);
      }

      if (structure[tagName] && typeof one[structure[tagName]] !== 'boolean') {
        one[structure[tagName]].appendChild(elem);
      }
      else if (curParentNode && curParentNode.appendChild) {
        curParentNode.appendChild(elem);
      }

      if (!unary) {
        elems.push(elem);
        curParentNode = elem;
      }
    },
    end: function(/* tag */) {
      elems.length -= 1;

      // Init the new parentNode
      curParentNode = elems[elems.length - 1];
    },
    chars: function(text) {
      curParentNode.appendChild(doc.createTextNode(text));
    },
    comment: function(/* text */) {
      // create comment node
    },
    ignore: function(/* text */) {
      // What to do here?
    }
  });

  return doc;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html-minifier.htmlparser.HTMLtoXML"></a>[function <span class="apidocSignatureSpan">html-minifier.htmlparser.</span>HTMLtoXML (html)](#apidoc.element.html-minifier.htmlparser.HTMLtoXML)
- description and source-code
```javascript
HTMLtoXML = function (html) {
  var results = '';

  new HTMLParser(html, {
    start: function(tag, attrs, unary) {
      results += '<' + tag;

      for (var i = 0, len = attrs.length; i < len; i++) {
        results += ' ' + attrs[i].name + '="' + (attrs[i].value || '').replace(/"/g, '&#34;') + '"';
      }

      results += (unary ? '/' : '') + '>';
    },
    end: function(tag) {
      results += '</' + tag + '>';
    },
    chars: function(text) {
      results += text;
    },
    comment: function(text) {
      results += '<!--' + text + '-->';
    },
    ignore: function(text) {
      results += text;
    }
  });

  return results;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html-minifier.tokenchain"></a>[module html-minifier.tokenchain](#apidoc.module.html-minifier.tokenchain)

#### <a name="apidoc.element.html-minifier.tokenchain.tokenchain"></a>[function <span class="apidocSignatureSpan">html-minifier.</span>tokenchain ()](#apidoc.element.html-minifier.tokenchain.tokenchain)
- description and source-code
```javascript
function TokenChain() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html-minifier.tokenchain.prototype"></a>[module html-minifier.tokenchain.prototype](#apidoc.module.html-minifier.tokenchain.prototype)

#### <a name="apidoc.element.html-minifier.tokenchain.prototype.add"></a>[function <span class="apidocSignatureSpan">html-minifier.tokenchain.prototype.</span>add (tokens)](#apidoc.element.html-minifier.tokenchain.prototype.add)
- description and source-code
```javascript
add = function (tokens) {
  var self = this;
  tokens.forEach(function(token) {
    var key = '$' + token;
    if (!self[key]) {
      self[key] = [];
      self[key].processed = 0;
    }
    self[key].push(tokens);
  });
}
```
- example usage
```shell
...
      var index;
      while ((index = tokens.indexOf(token)) !== -1) {
        tokens.splice(index, 1);
      }
      tokens.forEach(function(token) {
        self['$' + token].processed++;
      });
      chain.add(tokens.slice(0));
    });
    sorter[key] = chain.createSorter();
    return true;
  }
  return false;
});
return sorter;
...
```

#### <a name="apidoc.element.html-minifier.tokenchain.prototype.createSorter"></a>[function <span class="apidocSignatureSpan">html-minifier.tokenchain.prototype.</span>createSorter ()](#apidoc.element.html-minifier.tokenchain.prototype.createSorter)
- description and source-code
```javascript
createSorter = function () {
  var self = this;
  var sorter = new Sorter();
  sorter.keys = Object.keys(self).sort(function(j, k) {
    var m = self[j].length;
    var n = self[k].length;
    return m < n ? 1 : m > n ? -1 : j < k ? -1 : j > k ? 1 : 0;
  }).filter(function(key) {
    if (self[key].processed < self[key].length) {
      var token = key.slice(1);
      var chain = new TokenChain();
      self[key].forEach(function(tokens) {
        var index;
        while ((index = tokens.indexOf(token)) !== -1) {
          tokens.splice(index, 1);
        }
        tokens.forEach(function(token) {
          self['$' + token].processed++;
        });
        chain.add(tokens.slice(0));
      });
      sorter[key] = chain.createSorter();
      return true;
    }
    return false;
  });
  return sorter;
}
```
- example usage
```shell
...
            tokens.splice(index, 1);
          }
          tokens.forEach(function(token) {
            self['$' + token].processed++;
          });
          chain.add(tokens.slice(0));
        });
        sorter[key] = chain.createSorter();
        return true;
      }
      return false;
    });
    return sorter;
  }
};
...
```



# <a name="apidoc.module.html-minifier.utils"></a>[module html-minifier.utils](#apidoc.module.html-minifier.utils)

#### <a name="apidoc.element.html-minifier.utils.createMap"></a>[function <span class="apidocSignatureSpan">html-minifier.utils.</span>createMap (values, ignoreCase)](#apidoc.element.html-minifier.utils.createMap)
- description and source-code
```javascript
function createMap(values, ignoreCase) {
  var map = {};
  values.forEach(function(value) {
    map[value] = 1;
  });
  return ignoreCase ? function(value) {
    return map[value.toLowerCase()] === 1;
  } : function(value) {
    return map[value] === 1;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html-minifier.utils.createMapFromString"></a>[function <span class="apidocSignatureSpan">html-minifier.utils.</span>createMapFromString (values, ignoreCase)](#apidoc.element.html-minifier.utils.createMapFromString)
- description and source-code
```javascript
createMapFromString = function (values, ignoreCase) {
  return createMap(values.split(/,/), ignoreCase);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
