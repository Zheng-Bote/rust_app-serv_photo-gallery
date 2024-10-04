# Compilation from sources

<hr>

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

**Table of Contents**

- [Brief](#brief)
- [Compile and Linking](#compile-and-linking)
- [checkboxes](#checkboxes)
  - [markdown](#markdown)
  - [html](#html)
- [Artikel](#artikel)
  - [mit h2 Überschrift](#mit-h2-%C3%9Cberschrift)
  - [mit h2 Überschrift](#mit-h2-%C3%9Cberschrift-1)
- [Sektion](#sektion)
- [Artikel 2](#artikel-2)
  - [Text](#text)
  - [80 Text](#80-text)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

<hr>

# Brief

HowTo compile sources

# Compile and Linking

```Shell
cd src
conan install . --output-folder=../build --build=missing

cd ../build
cmake -S ../src -B . -G "Unix Makefiles" -DCMAKE_TOOLCHAIN_FILE=conan_toolchain.cmake  -DCMAKE_POLICY_DEFAULT_CMP0091=NEW -DCMAKE_BUILD_TYPE=Release

# cmake --build . --parallel <number of CPU cores>
cmake --build .

# generate Doxygen documentation with
cd build
cmake --build . --target doxygen

# packaging
cd build && sudo cpack -G "ZIP;DEB;RPM" -B packages
# or
cd build && sudo cmake --build . --target package

# packaging sources
cd build && sudo cmake --build . --target  package_source
```

# Description

just a test area, still uner construction

<p align="right">(<a href="#top">back to top</a>)</p>

# checkboxes

## markdown

- [x] this one should be checked
- [ ] this one is not checked

[x] this one should be checked
[ ] this one is not checked

## html

<input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
<label for="vehicle1"> I have a bike</label><br>
<input type="checkbox" id="vehicle2" name="vehicle2" value="Car" checked>
<label for="vehicle2"> I have a car</label><br>
<input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
<label for="vehicle3"> I have a boat</label>

<p align="right">(<a href="#top">back to top</a>)</p>

# Artikel

<article>
<h3>mit h2 Überschrift</h3>
<p>und p text</p>
</article>

# Sektion

<section>
<h3>mit h2 Überschrift</h3>
<p>und p text</p>
</section>

<section>
<h3>mit h2 Überschrift</h3>
<p>und p text</p>
</section>

# Artikel 2

<article>
<h3>Text</h3>

<p>
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
</p>

</article>

<article>
<h3>80 Text</h3>
<div class="text">
<p>
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

</p>
</div>
</article>

<p align="right">(<a href="#top">back to top</a>)</p>
