# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Variational generalized linear mixed effects regression Use vglmer With (In) R Software
install.packages("vglmer")
library("vglmer")
vglmer = read.csv("https://raw.githubusercontent.com/timbulwidodostp/vglmer/main/vglmer/vglmer.csv",sep = ";")
# Estimation Variational generalized linear mixed effects regression Use vglmer With (In) R Software
vglmer_binomial_1 <- vglmer(formula = y ~ x + (x | g), data = vglmer, family = 'binomial')
vglmer_binomial_1
summary(vglmer_binomial_1)
vglmer_binomial_2 <- vglmer(formula = y ~ v_s(x) + (x | g), data = vglmer, family = 'binomial')
vglmer_binomial_2
summary(vglmer_binomial_2)
vglmer_linear_1 <- vglmer(formula = y ~ x + (x | g), data = vglmer, family = 'linear')
vglmer_linear_1
summary(vglmer_linear_1)
vglmer_linear_2 <- vglmer(formula = y ~ v_s(x) + (x | g), data = vglmer, family = 'linear')
vglmer_linear_2
summary(vglmer_linear_2)
# Variational generalized linear mixed effects regression Use vglmer With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished