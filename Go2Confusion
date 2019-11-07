def Confusao(y,ypred):
  cm=np.array(pd.crosstab(y, ypred))
  TP = np.diag(cm) # true positive
  FP = np.sum(cm, axis=0) - TP # false positive
  FN = np.sum(cm, axis=1) - TP # false negative
  precision = TP/(TP+FP)
  recall = TP/(TP+FN)
  return cm, precision, recall
