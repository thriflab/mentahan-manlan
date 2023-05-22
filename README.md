# CodeIgniter 4 Framework

## What is CodeIgniter?

CodeIgniter is a PHP full-stack web framework that is light, fast, flexible and secure.
More information can be found at the [official site](https://codeigniter.com).

This repository holds the distributable version of the framework.
It has been built from the
[development repository](https://github.com/codeigniter4/CodeIgniter4).

More information about the plans for version 4 can be found in [CodeIgniter 4](https://forum.codeigniter.com/forumdisplay.php?fid=28) on the forums.

The user guide corresponding to the latest version of the framework can be found
[here](https://codeigniter4.github.io/userguide/).

## Important Change with index.php

`index.php` is no longer in the root of the project! It has been moved inside the *public* folder,
for better security and separation of components.

This means that you should configure your web server to "point" to your project's *public* folder, and
not to the project root. A better practice would be to configure a virtual host to point there. A poor practice would be to point your web server to the project root and expect to enter *public/...*, as the rest of your logic and the
framework are exposed.

**Please** read the user guide for a better explanation of how CI4 works!

## Repository Management

We use GitHub issues, in our main repository, to track **BUGS** and to track approved **DEVELOPMENT** work packages.
We use our [forum](http://forum.codeigniter.com) to provide SUPPORT and to discuss
FEATURE REQUESTS.

This repository is a "distribution" one, built by our release preparation script.
Problems with it can be raised on our forum, or as issues in the main repository.

## Contributing

We welcome contributions from the community.

Please read the [*Contributing to CodeIgniter*](https://github.com/codeigniter4/CodeIgniter4/blob/develop/CONTRIBUTING.md) section in the development repository.

## Server Requirements

PHP version 7.4 or higher is required, with the following extensions installed:

- [intl](http://php.net/manual/en/intl.requirements.php)
- [mbstring](http://php.net/manual/en/mbstring.installation.php)

Additionally, make sure that the following extensions are enabled in your PHP:

- json (enabled by default - don't turn it off)
- [mysqlnd](http://php.net/manual/en/mysqlnd.install.php) if you plan to use MySQL
- [libcurl](http://php.net/manual/en/curl.requirements.php) if you plan to use the HTTP\CURLRequest library

https://drive.google.com/drive/folders/11FORyBhu2aJGPhaXxFn21JpPbZY89CNB
KLKP
Minggu 3 = https://youtu.be/W8IFrEX_dZw
Minggu 4 = https://youtu.be/WLSpjrPB_HY 

<!--
@license
Copyright (c) 2016 The Polymer Project Authors. All rights reserved.
This code may only be used under the BSD style license found at http://polymer.github.io/LICENSE.txt
The complete set of authors may be found at http://polymer.github.io/AUTHORS.txt
The complete set of contributors may be found at http://polymer.github.io/CONTRIBUTORS.txt
Code distributed by Google as part of the polymer project is also
subject to an additional IP rights grant found at http://polymer.github.io/PATENTS.txt
-->

<link rel="import" href="../bower_components/polymer/polymer-element.html">
<link rel="import" href="shared-styles.html">

<dom-module id="my-view1">
  <template>
    <style include="shared-styles">
      :host {
        display: block;

        padding: 10px;
      }
    </style>

    <div class="card">
      <div class="circle">1</div>
      <h1>Registrasi</h1>
      <form action="">
        <label for="">Nama</label>
        <input type="text" placeholder="Nama" required>
        <label for="">Email</label>
        <input type="email" placeholder="Email" required>
        <label for="">Password</label>
        <input type="password" placeholder="Password" required>
        <label for="">Jenis Kelamin</label>
        <select name="jkel" id="jkel">
          <option value="Pilih">--Pilih Jenis Kelamin</option>
          <option value="pria"></option>
          <option value="wanita">Wanita</option>
        </select>

        <label for="">Alamat</label>
        <textarea name="alamat" id="" cols="30" rows="10" placeholder="Masukan Alamat" required></textarea>

        <input type="submit" value="Registrasi">
      </form>
    </div>
  </template>

  <script>
    class MyView1 extends Polymer.Element {
      static get is() { return 'my-view1'; }
    }

    window.customElements.define(MyView1.is, MyView1);
  </script>
</dom-module>
