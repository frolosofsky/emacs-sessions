#Simple session manager for emacs

This manager is build on the top of emacs desktop-* functionality. You can use it to save your sessions with different names. Phisically files will be saved in ~/.emacs.d/sessions folder by default.

##Installation

File `sessions.el` must be available from `load-path`.

##Usage

* `sessions-save` to save you session. If you haven't select session name yet emacs will ask you.
* `sessions-open` to open session. You can use auto complete session names.
* `sessions` to see all available sessions.
* `sessions-close` to close current session.
* `sessions-set-name` to set new name for your current session.

##.emacs

    (require 'sessions)
    ;; auto save on emacs exit
    ;; (add-hook 'kill-emacs-hook (lambda () (sessions-close)))
