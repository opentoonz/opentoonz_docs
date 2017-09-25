# OpenToonz User Manual

This repositry is for the documentation of OpenToonz, an open-source full-featured 2D animation creation software.
The documentation is written in [reStructuredText](http://docutils.sourceforge.net/rst.html) format, built with [Sphinx](http://www.sphinx-doc.org/en/stable/) and released via [Read the Docs](https://readthedocs.org/).

## Documentation URL
- [http://opentoonz.readthedocs.io](http://opentoonz.readthedocs.io)
- [http://opentoonz.rtfd.io](http://opentoonz.rtfd.io)

## How to Build Locally

- Acquire the Source
- Install [Python](https://www.python.org/downloads/)
- Install Sphinx

`$ pip install sphinx sphinx-autobuild`

- Install `sphinx_rtd_theme` theme

`$ pip install sphinx_rtd_theme`

- Build

`$ make html`

- The result HTML files will be generated under `build/html/`

## Internationalization (i18n) of the Manual

- Install i18n package

`$ pip install sphinx-intl`

- Generate the message catalogue (.pot)

`$ make gettext`

.pot files will be generated in `build/gettext` .

- Copy .pot to your language's locale folder

`$ sphinx-intl update -p build/gettext -l ja`

Please replace `ja` by the language you would like to translate. See [the sphinx manual](http://www.sphinx-doc.org/en/stable/config.html#confval-language) for supported languages.
Then .po files will be generated in `source/locale/ja/LC_MESSAGES`.

- To update .po to the latest version, do the same commands again;

```
$ make gettext
$ sphinx-intl update -p build/gettext -l ja
```
- Translate the document in .po files

In .po files, there are list of messages like:

```
#: ../../source/index.rst:7
msgid "OpenToonz User Manual"
msgstr ""
```

Input translation into `msgstr` like as follows:

```
#: ../../source/index.rst:7
msgid "OpenToonz User Manual"
msgstr "OpenToonz ユーザマニュアル"
```

Note: Make sure to maintain the syntax of reStructuredText in your translated text.

- Generate the translated-version HTML locally

`$ make SPHINXOPTS="-D language='ja'" html`

- To include the translation to the User Manual, some settings in Read the Docs is needed. Please let me (@shun-iwasawa) know when you firstly merge your language translation.

## Licensing

This documentation is published under a [CC-BY-NC 4.0 Int. License](https://creativecommons.org/licenses/by-nc/4.0/).

### Special Thanks

The documentation is based on Toonz 7.1 Harlequin Use Guide, originally created by Digital Video, S.p.A., Rome Italy
