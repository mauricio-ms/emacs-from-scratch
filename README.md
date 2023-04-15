# Commands
- M-x M-o -> List more options about the command
- C-h f   -> Describre function

# Key Bindings
Setting a function from a key binding:
```lisp
(global-set-key (kbd "C-M-j") 'counsel-switch-buffer)
```

Define a key for a specific key map:
```lisp
(define-key emacs-lisp-mode-map (kbd "C-x M-t") 'counsel-load-theme)
```

A more simpler way to define key bindings is using the General El package:
```lisp
(use-package general)

(general-define-key
 "C-M-j" 'counsel-switch-buffer)
```

# Evil Mode Commands

## Switch between Modes
i -> Insert Mode
ESC -> Vim Mode
C-z -> Emacs Mode

## Cursor Control
j -> Up Line
k -> Down Line
C-v -> Mark Lines
shift-5 -> Go to End Delimiter

## Buffer Control
q -> Close
dd -> Delete Line
u -> Undo

## Window Management
C-w v -> Vertical Split
C-w s -> Horizontal Split
C-w c -> Close Window
