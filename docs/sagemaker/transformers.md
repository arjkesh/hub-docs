# Transformers Images

[Transformers](https://huggingface.co/docs/transformers/en/index) provides APIs and tools to easily download and fine-tune state-of-the-art pretrained models, for use across NLP, computer vision, audio, and more.

Below, we include a list of the latest images available on AWS, which come pre-packaged with transformers and [datasets](https://huggingface.co/docs/datasets/en/index) libraries for your convenience. Check out some of the tutorials in the reference section for more information!

 To find the latest supported versions of the HF DLCs, check out https://aws.amazon.com/releasenotes/dlc-support-policy/

<!-- START AUTOGEN TABLE -->
## huggingface-pytorch-training

| Framework Version | Image Type | Image URI | Size (GB) | Pushed At | Details |
| --- | --- | --- | --- | --- | --- |
| 2.3 | gpu | `763104351884.dkr.ecr.us-west-2.amazonaws.com/huggingface-pytorch-training:2.3.0-transformers4.48.0-gpu-py311-cu121-ubuntu20.04-v2.1` | 8.75 | 2025-03-14 13:15:19 | [Details](https://github.com/aws/deep-learning-containers/blob/master/available_images.md#huggingface-training-containers) |
| 2.1 | gpu | `763104351884.dkr.ecr.us-west-2.amazonaws.com/huggingface-pytorch-training:2.1.0-transformers4.36.0-gpu-py310-cu121-ubuntu20.04-v1.2` | 8.75 | 2024-10-26 05:11:53 | [Details](https://github.com/aws/deep-learning-containers/blob/master/available_images.md#huggingface-training-containers) |


### SM Example
```
# create Hugging Face Model Class
huggingface_model = HuggingFaceModel(
	image_uri=get_huggingface_llm_image_uri("huggingface",version="2.3"),
	env=<insert_hub_obj>,
	role=<insert_role>, 
)

# deploy model to SageMaker Inference
predictor = huggingface_model.deploy(
	initial_instance_count=1,
	instance_type="ml.g6.48xlarge",
	container_startup_health_check_timeout=2400,
)
```
                          

## huggingface-pytorch-inference

| Framework Version | Image Type | Image URI | Size (GB) | Pushed At | Details |
| --- | --- | --- | --- | --- | --- |
| 2.3 | gpu | `763104351884.dkr.ecr.us-west-2.amazonaws.com/huggingface-pytorch-inference:2.3.0-transformers4.48.0-gpu-py311-cu121-ubuntu22.04-v2.1` | 9.12 | 2025-03-03 18:16:45 | [Details](https://github.com/aws/deep-learning-containers/blob/master/available_images.md#huggingface-inference-containers) |
| 2.3 | cpu | `763104351884.dkr.ecr.us-west-2.amazonaws.com/huggingface-pytorch-inference:2.3.0-transformers4.48.0-cpu-py311-ubuntu22.04-v2.1` | 1.39 | 2025-03-03 18:04:16 | [Details](https://github.com/aws/deep-learning-containers/blob/master/available_images.md#huggingface-inference-containers) |
| 2.1 | gpu | `763104351884.dkr.ecr.us-west-2.amazonaws.com/huggingface-pytorch-inference:2.1.0-transformers4.37.0-gpu-py310-cu118-ubuntu20.04-v1.4` | 9.07 | 2024-11-13 18:51:05 | [Details](https://github.com/aws/deep-learning-containers/blob/master/available_images.md#huggingface-inference-containers) |
| 2.1 | cpu | `763104351884.dkr.ecr.us-west-2.amazonaws.com/huggingface-pytorch-inference:2.1.0-transformers4.37.0-cpu-py310-ubuntu22.04-v1.4` | 2.13 | 2024-11-13 18:37:35 | [Details](https://github.com/aws/deep-learning-containers/blob/master/available_images.md#huggingface-inference-containers) |


### SM Example
```
# create Hugging Face Model Class
huggingface_model = HuggingFaceModel(
	image_uri=get_huggingface_llm_image_uri("huggingface",version="2.3"),
	env=<insert_hub_obj>,
	role=<insert_role>, 
)

# deploy model to SageMaker Inference
predictor = huggingface_model.deploy(
	initial_instance_count=1,
	instance_type="ml.g6.48xlarge",
	container_startup_health_check_timeout=2400,
)
```
                          

## huggingface-pytorch-inference-neuronx

| Framework Version | Image Type | Image URI | Size (GB) | Pushed At | Details |
| --- | --- | --- | --- | --- | --- |
| 2.1 | neuronx | `763104351884.dkr.ecr.us-west-2.amazonaws.com/huggingface-pytorch-inference-neuronx:2.1.2-transformers4.43.2-neuronx-py310-sdk2.20.0-ubuntu20.04-v2.1` | 7.57 | 2025-03-14 13:24:17 | [Details](https://github.com/aws/deep-learning-containers/blob/master/available_images.md#huggingface-inference-containers) |


### SM Example
```
# create Hugging Face Model Class
huggingface_model = HuggingFaceModel(
	image_uri=get_huggingface_llm_image_uri("huggingface",version="2.1"),
	env=<insert_hub_obj>,
	role=<insert_role>, 
)

# deploy model to SageMaker Inference
predictor = huggingface_model.deploy(
	initial_instance_count=1,
	instance_type="ml.g6.48xlarge",
	container_startup_health_check_timeout=2400,
)
```
                          

## huggingface-pytorch-training-neuronx

| Framework Version | Image Type | Image URI | Size (GB) | Pushed At | Details |
| --- | --- | --- | --- | --- | --- |
| 2.1 | neuronx | `763104351884.dkr.ecr.us-west-2.amazonaws.com/huggingface-pytorch-training-neuronx:2.1.2-transformers4.48.1-neuronx-py310-sdk2.20.0-ubuntu20.04-v2.0` | 13.44 | 2025-02-12 15:55:38 | [Details](https://github.com/aws/deep-learning-containers/blob/master/available_images.md#huggingface-training-containers) |


### SM Example
```
# create Hugging Face Model Class
huggingface_model = HuggingFaceModel(
	image_uri=get_huggingface_llm_image_uri("huggingface",version="2.1"),
	env=<insert_hub_obj>,
	role=<insert_role>, 
)

# deploy model to SageMaker Inference
predictor = huggingface_model.deploy(
	initial_instance_count=1,
	instance_type="ml.g6.48xlarge",
	container_startup_health_check_timeout=2400,
)
```
                          
<!-- END AUTOGEN TABLE -->