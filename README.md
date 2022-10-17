## English description

This repository contains a Jupyter notebook that work on simulated data using PySpark.

Data are split in equal halves, then for each one a linear model is estimated, and predictions for the response are obtained based on the model associated to the other split. The predictions are then used to perform the rank-one-out split conformal algorithm in order to build predictive intervals with desired empirical coverage. The operations are repeated for an additive model (estimated using penalized regression splines). In conclusion the models are compared based on their RMSE, in addition to average length and empirical coverage the of predictive intervals.

The two models are estimated using a MapReduce approach, implemented thanks to PySpark internal functions.

This analysis is the application on simulated data of the techniques developed for my M.Sc. thesis in Statistical Sciences, titled: "Managing Big Data on the cloud: review and applications".


## Italian description

Questa repository contiene un notebook Jupyter che lavora su dati simulati utilizzando PySpark.

I dati vengono divisi in metà uguali, quindi per ciascuna viene stimato un modello lineare e si ottengono le previsioni per la risposta in base al modello stimato associato all'altra suddivisione. Le previsioni vengono quindi utilizzate per eseguire l'algoritmo rank-one-out split conformal al fine di creare intervalli predittivi con copertura empirica desiderata. Le operazioni vengono ripetute anche per un modello additivo (stimato con splines di regressione penalizzate). In conclusione i due modelli vengono confrontati in base al loro RMSE, oltre alla lunghezza media e alla copertura empirica degli intervalli predittivi.

I due modelli sono stimati utilizzando un approccio MapReduce, implementato grazie alle funzioni interne di PySpark.

Questa analisi è l'applicazione su dati simulati delle tecniche sviluppate per il mio M.Sc. tesi in Scienze Statistiche, dal titolo: "Gestire Big Data nel cloud: panoramica e applicazioni".
