.. title: Main page
.. slug: index
.. date: 2017-09-09 23:39:43 UTC+02:00
.. has_math: true
.. category:
.. link:
.. description: test Nikola
.. type: text

.. .............................................................................
.. default-role:: code
.. role:: text-primary
.. role:: text-secondary
.. role:: text-success
.. role:: text-info
.. role:: text-warning
.. role:: text-danger
.. role:: html(raw)
    :format: html
.. .............................................................................


.. figure:: /images/nikola_tesla_quote.tn.jpg
    :target: /images/nikola_tesla_quote.jpg
    :align: right
    :figclass: thumbnail

    Nikola Tesla, one of the greatest inventors ever.

Test site built with `Nikola <http://getnikola.com/>`_.

Het is niet nodig te hopen om te ondernemen, noch te slagen om te
volharden.
We must therefore glean up our experiments in this science from
a cautious observation of human life, and take them as they
appear in the common course of the world, by men’s behaviour in
company, in affairs, and in their pleasures. Where experiments
of this kind are judiciously collected and compared, we may hope
to establish on them a science, which will not be inferior in
certainty, and will be much superior in utility to any other of
human comprehension.

inline math with \\displaystyle :math:`\displaystyle\frac{\sum_{t=0}^{N}f(t,k) }{N}` and so

Example item list
=================

.. class:: li-smallskip

    - Both blog posts and non-blog pages can be included.

    - math formulas with TeX-like syntax can be used

    - **Jupyter** notebooks can be published. :text-info:`Jupyter is a
      very handy web application that allows you to create and share
      documents containing live code, equations, visualizations and
      explanatory text. It supports many languages including Python,
      which makes it a perfect tool for writing scientific articles.`

    - text-primary  :text-primary:`Jupyter is a very handy web application`

    - text-success  :text-success:`Jupyter is a very handy web application`

    - text-info  :text-info:`Jupyter is a very handy web application`

    - text-warning  :text-warning:`Jupyter is a very handy web application`

    - text-danger  :text-danger:`Jupyter is a very handy web application`

.. TEASER_END

Math examples
=============

Side note: :text-info:`An example how Nikola can render math using MathJax plugin. You can right-click the equation, get menu and see the TeX code (Show Math As - TeX Commands). Apropos, these are the famous Maxwell's equations describing electromagnetic field, probably one of the most favourite equations of Nikola Tesla :)`

.. math::
    \nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} & = \frac{4\pi}{c}\vec{\mathbf{j}} \\
    \nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\
    \nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\
    \nabla \cdot \vec{\mathbf{B}} & = 0


Options example
---------------

Option pros and cons |par|
    .. class:: pros-list

        - pro text 1

        - pro text 2
    .. class:: cons-list

        - con text 1

        - con text 2

Header 1
======================

.. figure:: /images/nikola_tesla_quote2.tn.jpg
    :target: /images/nikola_tesla_quote2.jpg
    :align: right
    :figclass: thumbnail

    Nikola Tesla in his laboratory.

Het is niet nodig te hopen om te ondernemen, noch te slagen om te
volharden.
We must therefore glean up our experiments in this science from
a cautious observation of human life, and take them as they
appear in the common course of the world, by men’s behaviour in
company, in affairs, and in their pleasures. Where experiments
of this kind are judiciously collected and compared, we may hope
to establish on them a science, which will not be inferior in
certainty, and will be much superior in utility to any other of
human comprehension.

Header 2
------------------------------------

Example ``code block``:

.. code::

    [themes]
        [mytheme]
            [assets]
                [css]
                    bootstrap.css
                    bootstrap.min.css
                    custom.css
                    nikola_ipython.css
                    theme.css
                [img]
                [js]
                    custom.js
            [templates]
                base.tmpl
            bundles
            parent

MathJax vs. KaTeX
-----------------

There are basically two options for rending math. `MathJax <https://www.mathjax.org/>`_ is the default option for Nikola and also for Jupyter notebooks.

On the other side, `KaTeX <https://github.com/Khan/KaTeX>`_ seems to be much faster to render, and there is no obvious re-rendering after page reloading. The font quality is also nice or maybe even better than MathJax. But I have faced serious problems that made me give up using KaTeX for my site. For example, I wasn't able to insert inline math using standard `$..$` directive, and TeX environments produced by Nikola are also not supported. All this makes KaTeX still too immature for usage with Nikola and Jupyter.

Python code block
-----------------

.. code:: python

    GITHUB_DEPLOY_BRANCH = 'master'  # Deploy the Nikola output to the master branch of your repository
    GITHUB_SOURCE_BRANCH = 'src'     # Deploy Nikola project source files to src branch of your repository
    GITHUB_COMMIT_SOURCE = True

Console code block
------------------

.. code:: console

    $ git config --global user.name "USER_NAME"
    $ git config --global user.email "USER_EMAIL"
    $ git init

Conclusion
==========

That's all.

.. |br| raw:: html

   <br />

.. |par| raw:: html

   <p />
