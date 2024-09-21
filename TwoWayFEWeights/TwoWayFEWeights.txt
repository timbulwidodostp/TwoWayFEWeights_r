# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Estimation of the weights attached to the two-way fixed effects regressions Use twowayfeweights With (In) R Software
# Estimates the weights attached to the two-way fixed effects regressions studied in de Chaisemartin & D'Haultfoeuille (2020a), as well as summary measures of these regressions' robustness to heterogeneous treatment effects Use twowayfeweights With (In) R Software
install.packages("TwoWayFEWeights")
library("TwoWayFEWeights")
TwoWayFEWeights = read.csv("https://raw.githubusercontent.com/timbulwidodostp/TwoWayFEWeights_r/main/TwoWayFEWeights/TwoWayFEWeights.csv",sep = ";")
# Estimation of the weights attached to the two-way fixed effects regressions Use twowayfeweights With (In) R Software
# Estimates the weights attached to the two-way fixed effects regressions studied in de Chaisemartin & D'Haultfoeuille (2020a), as well as summary measures of these regressions' robustness to heterogeneous treatment effects Use twowayfeweights With (In) R Software
twowayfeweights_1 <- twowayfeweights(TwoWayFEWeights, "lwage", "nr", "year", "union", type = "feTR", summary_measures = TRUE, test_random_weights = "educ")
print(twowayfeweights_1)
twowayfeweights_2 <- twowayfeweights(TwoWayFEWeights,"diff_lwage", "nr", "year", "diff_union", type = "fdTR", "union", summary_measures = TRUE, test_random_weights = "educ")
print(twowayfeweights_2)
# Estimation of the weights attached to the two-way fixed effects regressions Use twowayfeweights With (In) R Software
# Estimates the weights attached to the two-way fixed effects regressions studied in de Chaisemartin & D'Haultfoeuille (2020a), as well as summary measures of these regressions' robustness to heterogeneous treatment effects Use twowayfeweights With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished