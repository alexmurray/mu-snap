![mu logo](https://www.gnu.org/software/emacs/images/emacs.png "mu")

# mu #

-------------------------------------------------------------------------------

**mu in a snap**

[![mu](https://snapcraft.io/maildir-utils/badge.svg)](https://snapcraft.io/maildir-utils)
[![mu](https://snapcraft.io/maildir-utils/trending.svg?name=0)](https://snapcraft.io/maildir-utils)

## Installation ##

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/maildir-utils)

``` shell
sudo snap install maildir-utils
```

## Configuration ##

To use `mu4e` within Emacs, you need to update the load-path using either
of the following methods:

### `use-package`

We recommend to use [use-package](https://github.com/jwiegley/use-package)

```emacs-lisp
(use-package mu4e
  :load-path "/snap/maildir-utils/current/share/emacs/site-lisp/mu4e/""
  ;; usual configuration here...
  )
```

### Manual

```emacs-lisp
(add-to-list 'load-path "/snap/maildir-utils/current/share/emacs/site-lisp/mu4e/")
(require mu4e)
;; usual configuration here...
```
