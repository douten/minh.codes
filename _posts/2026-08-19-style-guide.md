---
layout: default
title: Style Guide
code_highlight: true
---

Reference
{:.eyebrow}

# Style Guide

A living reference for the type scale, spacing tokens, and code styling in this design system. Every element below is rendered with the classes it documents.
{:.lead}

---

## Typography

---

Display
{:.display}

# Heading level 1

## Heading level 2

### Heading level 3

#### Heading level 4

This is the lead paragraph — larger and muted to introduce a section.
{:.lead}

This is default body copy. Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit.

Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem.

This is small text for secondary UI copy. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam.
{:.small}

This is micro text for metadata and labels. Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse.
{:.micro}

This is legal text for fine print. Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime placeat.
{:.legal}

Eyebrow Label. The eyebrow sits above a heading as a small uppercase overline. Uses `--tracking-wide` and the muted color.
{:.eyebrow}

---

## Spacing

The spacing scale runs from `--space-xs` (4px) to `--space-3xl` (80px). The blocks below show each step at scale.

<div style="background: var(--color-primary); height: var(--space-xs); border-radius: var(--radius-sm);"></div>

`--space-xs` — 4px — inline gaps, icon nudges
{:.micro}

<div style="background: var(--color-primary); height: var(--space-sm); border-radius: var(--radius-sm); margin-top: var(--space-md);"></div>

`--space-sm` — 8px — label to input, chip padding
{:.micro}

<div style="background: var(--color-primary); height: var(--space-md); border-radius: var(--radius-sm); margin-top: var(--space-md);"></div>

`--space-md` — 16px — default element gap
{:.micro}

<div style="background: var(--color-primary); height: var(--space-lg); border-radius: var(--radius-sm); margin-top: var(--space-md);"></div>

`--space-lg` — 24px — card padding, stack gap
{:.micro}

<div style="background: var(--color-primary); height: var(--space-xl); border-radius: var(--radius-sm); margin-top: var(--space-md);"></div>

`--space-xl` — 32px — between components
{:.micro}

<div style="background: var(--color-primary); height: var(--space-2xl); border-radius: var(--radius-sm); margin-top: var(--space-md);"></div>

`--space-2xl` — 48px — sub-section breaks
{:.micro}

<div style="background: var(--color-primary); height: var(--space-3xl); border-radius: var(--radius-sm); margin-top: var(--space-md);"></div>

`--space-3xl` — 80px — between page sections
{:.micro}

---

## Code

### Inline

Reference a token inline like `--space-md` or a property like `box-shadow`. Inline code uses the mono stack at `0.9em`.

### Fenced blocks

SCSS:

{% highlight scss %}
.card {
  padding: var(--space-lg);
  border: 1px solid var(--color-border);
  border-radius: var(--radius-base);
  box-shadow: var(--shadow-base);

  &:hover {
    box-shadow: var(--shadow-lg);
    transition: box-shadow var(--duration-base) var(--ease-out);
  }
}
{% endhighlight %}

HTML:

{% highlight html %}
<article class="card">
  <p class="eyebrow">Featured</p>
  <h3>Card title</h3>
  <p class="small">Supporting copy sits here.</p>
  <a href="#">Read more</a>
</article>
{% endhighlight %}

JavaScript:

{% highlight javascript %}
const cards = document.querySelectorAll(".card");

cards.forEach((card) => {
  card.addEventListener("click", () => {
    card.classList.toggle("is-active");
  });
});
{% endhighlight %}

Shell:

{% highlight console %}
rougify style github > _syntax.scss
bundle exec jekyll serve --livereload
{% endhighlight %}

---

## Links, lists, and quotes

Body copy can contain [inline links](#) that pick up `--color-primary` and shift to `--color-primary-hover` on hover.

Unordered list:

- Lorem ipsum dolor sit amet
- Consectetur adipiscing elit
- Sed do eiusmod tempor incididunt

Ordered list:

1. Ut enim ad minim veniam
2. Quis nostrud exercitation
3. Ullamco laboris nisi

> Blockquotes carry a longer aside. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit.
