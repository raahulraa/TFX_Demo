# Model Signature

I have created successfully the model signature for keras, Xgboost, and sckit-learn models using Tensorflow Extended.

For PyTorch, there are different libraries. No Libraries we can completely use it.
1. TorchX: it is mainly used to push the trainer code to the K8 cluster, but it is not providing any model signatures.
2. Ray: It is mainly used to set up the cluster and GPU parallelization. but again no sihnature.
3. ZenML: We may need to add customization logic to use the model signature.

Review with PY:
TFX is using Google MLMD underneath the TFX pipelines, So all the details are stored in the MLMD. We have a Registry database similar to MLMD. So shortly we will implement metadata and will store it in the trained version table. So the details can be shown on the UI and model endpoint API call.
