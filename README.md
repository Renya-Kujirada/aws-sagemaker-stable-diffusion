# sagemaker-stable-diffusion


## link
- [original notebook](https://github.com/aws/amazon-sagemaker-examples/blob/main/inference/generativeai/llm-workshop/lab2-stable-diffusion/option1-jumpstart/BONUS_Amazon_JumpStart_Upscaling.ipynb)
- [pretrained model table](https://sagemaker.readthedocs.io/en/stable/doc_utils/pretrainedmodels.html#)

## memo

- 実行情報
```
endpoint_name: jumpstart-example-model-upscaling-stabi-2023-08-21-13-38-40-357
inference_instance_type: ml.p3.2xlarge
deploy_image_uri: 763104351884.dkr.ecr.ap-northeast-1.amazonaws.com/huggingface-pytorch-inference:1.10.2-transformers4.17.0-gpu-py38-cu113-ubuntu20.04
model_uri: s3://jumpstart-cache-prod-ap-northeast-1/stabilityai-infer/prepack/v1.0.0/infer-prepack-model-upscaling-stabilityai-stable-diffusion-x4-upscaler-fp16.tar.gz
model: <sagemaker.model.Model object at 0x7f353ca89a90>
model_predictor: Predictor: {'endpoint_name': 'jumpstart-example-model-upscaling-stabi-2023-08-21-13-38-40-357', 'sagemaker_session': <sagemaker.session.Session object at 0x7f35341039d0>, 'serializer': <sagemaker.base_serializers.IdentitySerializer object at 0x7f34f35672e0>, 'deserializer': <sagemaker.base_deserializers.BytesDeserializer object at 0x7f34f3567340>}
```

- より大きな画像を超解像する場合は，以下のインスタンスを利用するよう推奨されている
```
ml.g5.2xlarge
```
