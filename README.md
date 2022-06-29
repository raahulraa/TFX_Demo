# Model Signature

I have created successfully the model signature for keras, xgboost and sckit learn models using Tensorflow Extended.

For pytorch, there are diffrent libraries. No Libraris we can completely use it.
1. TorchX : it is mainly used to push the trinaer code to the K8 cluster, but it is not providing any model signatures.
2. Ray : It is mainly used to set up the clusester and GPU parallisation. but again no sihnature.
3. ZenML : We may need to add customization logic to use model signature.

Review with PY:
TFX is using Google MLMD underneath the TFX pipelines, So all the details are stored in the MLMD.We have Registry database similar like MLMD. So in the near future we will implement a metadata and will store in the trained version table. So the details can be shown on the UI and model endpoint api call.
