# Cyber Cafe Theme for Emacs

Cyber Cafe is an almost colorless, white-on-black theme. Created for
distraction-less programming, knowing that syntax highlight is overrated.

![screenshot](screenshot.png)

## Installation

I have a [melpa recipe](https://github.com/melpa/melpa/pull/8717) pull-requested
but it probably won't be merged.

Personally I like to manually install it opening the `cybercafe-theme.el` file
and running `package-install-from-buffer`. Them `use-package` will just works:

```elisp
(use-package cybercafe-theme
  :config
  (setq cybercafe-cyberpunk nil) ;; set this to `t` to use more
                                 ;; green. Personally I like it!
  (load-theme 'cybercafe t))
```

## Customizing

Currently there's two customizable options: if you set the variable
`cybercafe-cyberpunk` to non-nil before applying the theme, more green will be
used to UI components. And if you set `cybercafe-soft`, a slighter lighter
background will be used.

## Compatibility

I've only added special support for stuff I use. Feel free to contribute support
for other modes. Most should work just with the `font-lock` support tho.

- Magit  
- Ido  
- Dired  
- Org  
- Markdown  
- Tuareg  
- Doom Modeline  
