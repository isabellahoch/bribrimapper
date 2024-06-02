=============
Bribri Mapper
=============

.. image:: https://badge.fury.io/py/bribrimapper.svg
    :target: https://pypi.org/project/bribrimapper

.. image:: https://github.com/isabellahoch/bribrimapper/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/isabellahoch/bribrimapper/actions/workflows/ci.yml

Bribri Mapper is a Python library that provides identification and conversion
functions for Chinese text processing.

* Documentation: https://isabellahoch.github.io/bribrimapper/
* GitHub: https://github.com/isabellahoch/bribrimapper
* Free software: MIT license

Features
--------

* Convert between Chinese characters, Pinyin, Zhuyin, and the International
  Phonetic Alphabet.
* Identify a string as Traditional or Simplified Chinese, Pinyin, Zhuyin, or
  the International Phonetic Alphabet.

.. code:: python

    >>> s = '我是一个美国人。'
    >>> bribrimapper.hanzi.is_simplified(s)
    True
    >>> bribrimapper.hanzi.to_pinyin(s)
    'wǒshìyīgèměiguórén。'
    >>> bribrimapper.hanzi.to_pinyin(s, all_readings=True)
    '[wǒ][shì/shi/tí][yī][gè/ge/gě/gàn][měi][guó][rén/ren]。'

.. code:: python

    >>> s = 'Wǒ shì yīgè měiguórén.'
    >>> bribrimapper.transcriptions.is_pinyin(s)
    True
    >>> bribrimapper.transcriptions.pinyin_to_zhuyin(s)
    'ㄨㄛˇ ㄕˋ ㄧ ㄍㄜˋ ㄇㄟˇ ㄍㄨㄛˊ ㄖㄣˊ.'
    >>> bribrimapper.transcriptions.pinyin_to_ipa(s)
    'wɔ˧˩˧ ʂɨ˥˩ i˥ kɤ˥˩ meɪ˧˩˧ kwɔ˧˥ ʐən˧˥.'

Getting Started
---------------
* `Install Bribri Mapper <https://isabellahoch.github.io/bribrimapper/installation.html>`_
* Read `Bribri Mapper's tutorial <https://isabellahoch.github.io/bribrimapper/tutorial.html>`_
* Report bugs and ask questions via `GitHub Issues <https://github.com/isabellahoch/bribrimapper>`_
* Refer to the `API documentation <https://isabellahoch.github.io/bribrimapper/api.html>`_ when you need more technical information
* `Contribute <https://isabellahoch.github.io/bribrimapper/contributing.html>`_ documentation, code, or feedback
