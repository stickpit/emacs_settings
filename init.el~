;; package
(require 'package)
(add-to-list 'package-archives '("melpa" . "http://melpa.milkbox.net/packages/") t)
(add-to-list 'package-archives '("marmalade" . "http://marmalade-repo.org./packages/"))
(package-initialize)

;; org
(global-set-key "\C-cl" 'org-store-link)
(global-set-key "\C-cc" 'org-capture)
(global-set-key "\C-ca" 'org-agenda)
(global-set-key "\C-cb" 'org-iswitchb)
(setq org-todo-keywords '((type "TODO(t)" "WAITING(w)" "|" "DONE(d)" "REFERENCE(r)")))
(setq org-capture-templates
      '(("n" "Note" plain (file+headline "~/Documents/gtd.org" "Inbox")
	 "")))
(org-babel-do-load-languages
 'org-babel-load-languages '((python . t)))

;; semantic
(semantic-mode 1)
(global-semantic-idle-scheduler-mode 1)
(global-semantic-highlight-func-mode 1)
(global-semantic-decoration-mode 1)
(global-semantic-stickyfunc-mode 1)
(global-semantic-mru-bookmark-mode 1)

;;helm
(require 'helm-config)
(helm-mode 1)

;;yasnippet
(require 'yasnippet)
(yas-global-mode 1)

;;auto-complete
(ac-config-default)

;;expand-region
(require 'expand-region)
(global-set-key (kbd "C-^") 'er/expand-region)

;;flycheck
(add-hook 'after-init-hook #'global-flycheck-mode)

;;multiple-cursors
(require 'multiple-cursors)
(global-set-key (kbd "C-c t a") 'mc/edit-lines)
