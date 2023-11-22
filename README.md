# Brian Drake

## Copyright waiver

Most works are [automatically covered by copyright](
    https://alacc.org.au/faqs/#panel-137
),
but
all of this user's original GitHub contributions
are dedicated to the public domain
(no copyright)
under
the [CC0
    1.0
    Public Domain Dedication](
        https://creativecommons.org/publicdomain/zero/1.0/
    ),
a copy of which is in [LICENSE.txt](
    LICENSE.txt
).

## Freedom

All of this user's GitHub contributions
(including third party material,
except some quotes)
are libre
(or 'free as in freedom').
This means that they provide the public
[basic freedoms](
    https://www.fsf.org/about/what-is-free-software
);
these are the freedom to:
* Use the material for any purpose.
* Study and change the material.
* Distribute the material
  (with or without changes).

These freedoms are provided automatically,
with minimal requirements
(such as attribution),
and
can only be revoked for a particular user if that user violates those
requirements.
Material that denies the public these freedoms is called 'proprietary'.

## Software standards

All of this user's software meets,
and all software should meet,
the general standards below.

Somn commonly accepted software does not meet these standards;
in some cases,
examples are given below.

### Clarity

* Code
  (including
  APIs
  and
  automatically generated code)
  is
  self-documenting
  and
  works the way that type of code would be expected to work
  (where possible).
    
    A good example of unclear automatically generated code that turned out to
    be problematic is [Emscripten's glude code](
      https://hacks.mozilla.org/2019/03/standardizing-wasi-a-webassembly-system-interface/
    ).
* Dependencies are clearly stated.
    
    Static imports are placed together in a typical location.
    For dynamic imports triggered by function calls or similar constructs
    (like [in JavaScript](
      https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/import
    )),
    if the import specifier
    (just not the timing of the import)
    is known in advance,
    then the function call is wrapped in another function
    and
    the wrapper function's definition is placed together with any static
    imports.
    
    An example of dynamic imports that are typically not placed together with
    static imports is [lazily loaded Vue Router components](
      https://router.vuejs.org/guide/advanced/lazy-loading.html
    ).

### Modularisation

* Each part is as universal as possible
  (in particular,
  JavaScript code
  is [isomorphic](
    https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules#authoring_isomorphic_modules
  )
  and
  uses [strict mode](
    https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode
  )).

### Security

* Software is secure by default.
  In particular:
    
    * Software,
      by default,
      respects existing security boundaries,
      including those between operating system users.
      In particular:
        
        * Software creates temporary files
          (and directories)
          securely.
        * Software properly handles the possibility of local web servers being
          accessed by other local users.
    * Software does not access the network,
      except as necessary to follow the commands it is given.
* Recommendations given in documentation are secure.

### Support

* All versioned material uses [semantic versioning](
    https://semver.org/
  ).
* For all supported material,
  all critical issues
  (including security issues)
  are fixed via minimal patches as soon as practical.

## Support

For all current
(not archived)
GitHub repositories,
the latest release version is supported to the extent possible.
No level of support is actually guaranteed;
this user supports these repositories in their limited free time.

Forks are only included if they indicate that this user has taken responsibility
for them.
