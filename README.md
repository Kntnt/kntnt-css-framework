# Kntnt CSS Framework

*Kntnt CSS Framework* (*KCF*) is a comprehensive set of stylsheets that makes it easier to build web sites.

## Background

There are many CSS frameworks and similar solutions out there. The arguably most known is [Bootstrap](https://getbootstrap.com/). It's a fantastic toolkit "featuring Sass variables and mixins, responsive grid system, extensive prebuilt components, and powerful JavaScript plugins.

For better or worse, KCF is far from being as complete and competent as Bootstrap. KCF is focusing on providing a foundation with sane defaults that can be overridden with pure CSS and useful classes that can be used to accomplish everyday tasks.

## What it is

KCF is a set of cascading style sheets (CSS) that together make it possible to build a website relatively quickly by chiefly overriding default values and using classes.

The framework can be used with [Oxygen Builder](https://oxygenbuilder.com/) for WordPress. But there is no dependency or other connection to that tool at all, so it works perfectly with other tools or for writing code by hand.

Kntnt CSS Framework is developed by [Kntnt](https://www.kntnt.se) – a Swedish sales, marketing and web technology agency.

## How to use it

The document root must have following content:

    <body>
      <header>…</header>
      ⋮
      <main>…</main>
      ⋮
      <footer>…</footer>
    </body>

The `⋮` before and after `<main>…</main>` represents optional content that is *not unique* for the page. Typically, the first `⋮` is used for a important message shown on all pages, while the last `⋮` is used for gallery with related articles and similar. The `…` between `<main>` and `</main>` represents mandotary content that *is unique* for the page. Both `…` between `<main>` and `</main>` and non-emty `⋮` must have following structure:

    <div>
      <section>
        <div>CONTENT OF SECTION 1 IN DIV 1</div>
      </section>
      ⋮
      <section>
        <div>CONTENT OF SECTION i IN DIV 1</div>
      </section>
    </div>
    ⋮
    <div>
      <section>
        <div>CONTENT OF SECTION 1 IN DIV 2</div>
      </section>
      ⋮
      <section>
        <div>CONTENT OF SECTION j IN DIV n</div>
      </section>
    </div>

Any semantic element (`<section>`, `<aside>`, `<article>` and `<nav>`), can be used where `<section>` is used above. If no semantic element can be used in [inteded way](https://www.smashingmagazine.com/2013/01/the-importance-of-sections/), use `<div>` instead.

Replace `…` between in `<header>…</header>` and `<footer>…</footer>` with following content:

    <div>
      <div>CONTENT OF ROW 1</div>
    </div>
    <div>
      <div>CONTENT OF ROW 2</div>
    </div>

In the header, the first `…` is the topbar's content (e.g. with shortcut links to essential pages), and the second `…` is the content of the actual header (w.g. with logo and navigation).

In the footer, the first `…` is the actual footer's content (e.g. with sitemap and social media icons), and the second `…` is the content of the bottombar (e.g. with copyright notice and legal disclaimers).

Replace `…` with nothing (i.e. `<div></div>`) to disable a rows in in `<header>…</header>` or `<footer>…</footer>`.