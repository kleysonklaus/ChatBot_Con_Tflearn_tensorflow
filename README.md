# ChatBot_Con_Tflearn_tensorflow
 bot recomendador de peliculas utilizando la libreria tflearn de tensorflow
 
# intrucciones para utilizar:
nota: el codigo esta ejecutado desde el entorno Jupyter de ANACONDA, asi que es recomendable utilizarlo
- abrir el archivo "prueba_tensorflow.ipynb" desde Jupyter
- en el codigo se tendra que referencias los "intents.json", en caso se desea suministrar otro data set
- PARA OTRO DATA SET: se tiene que realizar un entrenamiento, para esto se tiene que descomentar el siguiente codigo
    
    ### model.fit(training, output, n_epoch = 100 , batch_size = 8, show_metric = True)
    ### model.save("save_model/model.tflearn")
    
- y comentar el siguiente codigo
    ###try:\n,
    ###       model.load(\"save_model/model.tflearn\")
    ###       print (\"recargado!\")
    ###   except:
    ###       model.fit(training, output, n_epoch = 500 , batch_size = 8, show_metric = True)
    ###       model.save(\"save_model/model.tflearn\")

- una ves entrenado todo se tiene que volver a comentar y descomentar lo que al inicio no lo estaba.
- para el data set de peliculas, solo se tiene que seguir la misma estructura, y claro referenciar en el codigo el PATH

