# Ctags

## Commands
  - PHP
    - `ctags -f ./wp-content/themes/light/TAGS -e -h \".php\" -R --exclude=\"\.git\" --totals=yes --tag-relative=yes --PHP-kinds=+cf --regex-PHP='/abstract class ([^ ]*)/^A/c/' --regex-PHP='/interface ([^ ]*)/^A/c/' --regex-PHP='/(public |static |abstract |protected |private )+function ([^ (]*)/^B/f/'`
