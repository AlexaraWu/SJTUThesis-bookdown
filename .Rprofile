options(bookdown.render.file_scope = FALSE)

if (.Platform$OS.type == 'windows') Sys.setlocale(, 'Chinese')

local({
  cmd <- "kpsewhich --var-value TEXINPUTS"
  sys_texinputs <- system(cmd, intern = TRUE, ignore.stderr = TRUE)
  local_texinputs <- "./texmf//"
  sys_sep <- .Platform$path.sep
  Sys.setenv(TEXINPUTS = paste(local_texinputs, sys_texinputs, sep = sys_sep))
})
