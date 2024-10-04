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

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

<hr>

# Brief

HowTo compile sources

# Compile and Linking

```Shell
cd build
cmake --build .
cmake --install
```

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

# Artikel

<article>
<h2>mit h2 Überschrift</h2>
<p>und p text</p>
</article>

<article>
## mit raute Überschrift

und text

</article>

# Sektion

<section>
<h2>mit h2 Überschrift</h2>
<p>und p text</p>
</section>

<section>
## mit raute Überschrift

und text

</section>
