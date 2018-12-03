```vim
" from
Send_keys_to_Tmux('"'.escape(a:text, '\"$').'"')
" to
Send_keys_to_Tmux('"'.escape(a:text, '\"$`').'"')

" To keep '`' when sending text to haskell (ghci) repl, e.g.:
Send_keys_to_Tmux('"'.escape("f `fmap` Just 3", '\"$`').'"')
```
