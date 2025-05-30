# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# M-Quantile Regression Coefficients Modeling Use iMqr (Mqrcm) With (In) R Software
install.packages("Mqrcm")
library("Mqrcm")
iMqr = read.csv("https://raw.githubusercontent.com/timbulwidodostp/iMqr/main/iMqr/iMqr.csv",sep = ";")
# Estimation M-Quantile Regression Coefficients Modeling Use iMqr (Mqrcm) With (In) R Software
y <- iMqr$y
x <- iMqr$x
model <- iMqr(y ~ x, formula.p = ~ p + I(p^2))
summary(model)

summary(model, p = c(0.1,0.2,0.3))
# M-Quantile Regression Coefficients Modeling Use iMqr (Mqrcm) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished