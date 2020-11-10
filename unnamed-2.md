> do this: mmm-mode and polymode. We decided to try out both of
> them...

The simple and direct approach is to install [mmm-mode][3] and add something like this to your `.emacs` file or equivalent:

```lisp
(require 'mmm-mode)
(setq mmm-global-mode 'maybe)

(mmm-add-classes
 '((markdown-python
     :submode python-mode
     :front "^```python[\r\n]+"
     :back "^```$")))
     
(mmm-add-mode-ext-class 'markdown-mode nil 'markdown-python)
```
