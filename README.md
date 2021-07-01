# MLOps-Jupyter-Templates

# Why Jupyter Templates?
There are many code based MLOps frameworks, such as Tensorflow Extended and Kubeflow. You have to check the tutorial, reference a lot to build your pipeline. Although the code is easy, the coding is boring and annoying.

At the same time, there are some GUI based MLOps services, such as GCP Vertex AI service. But the functions are limited and lacking flexibility.

A code based MLOps template can combine the advantages of code and GUI together.

1.All functions are implemented by code so that the following modification is easy. And the code can be continuously improved. 

2.Some pre-built charts and comments can make the code easy to understand.

So, I prefer code based MLOps templates. Technically and conveniently, I mean Jupyter notebook based templates.

# Which MLOps framework?
I used TFX, Kubeflow, GCP Vertex AI and AWS Sage Maker before.

Kubeflow is the most flexible, but the most heavy one. Unless you are willing to spend much time on infrastructure managing, I don't suggest setting up Kubeflow environment on your own.

TFX has more features and is tightly bundled with Tensorflow. At the same time, TFX can run in a normal Jupyter notebook. If you use Tensorflow, it's very convenient to use TFX.

GCP Vertex is serverless service, which can run Kubeflow code and TFX code under the hood.

AWS Sage Maker is similar to GCP Vertex AI, which has less features.

I will focus on TFX and Kubeflow code.

# TFX vs Kubeflow
According to the official guidance (https://cloud.google.com/vertex-ai/docs/pipelines/build-pipeline):

## Which pipelines SDK should I use?
Vertex Pipelines can run pipelines built using the Kubeflow Pipelines SDK v1.6 or higher, or TensorFlow Extended v0.30.0 or higher.

If you use TensorFlow in an ML workflow that processes terabytes of structured data or text data, we recommend that you build your pipeline using TFX.

To learn more about building a TFX pipeline, follow the TFX getting started tutorials.
To learn more about using Vertex Pipelines to run a TFX pipeline, follow the TFX on Google Cloud tutorials.

For other use cases, we recommend that you build your pipeline using the Kubeflow Pipelines SDK. By building a pipeline with the Kubeflow Pipelines SDK, you can implement your workflow by building custom components or reusing prebuilt components, such as the Google Cloud pipeline components. Google Cloud pipeline components make it easier to use Vertex AI services like AutoML in your pipeline.
The real two options: (Kubeflow on GCP Vertex AI) and (TFX on Jupyter Notebook)
Generally speaking, TFX is a light solution for Tensorflow based solution. (Kubeflow on GCP Vertex AI) is a heavy but flexible solution.

## TFX can run independent of GCP
Of course, as the official guidance said you may run TFX on GCP Vertex AI. But TFX can run independently.

# Credit
I will collect and improve good MLOps templates CONTINOUSLY here. I will mention all the original authors.

# A Fluent MLOps template for Time Series Data

It is worth mentioning that I have another related repo, 
https://github.com/MRYingLEE/DeepTime-Deep-Learning-Framework-for-Time-Series-Forecasting. 

That repo reflects my idea on MLOps with time series data. 
I expect a fluent and flexible MLOps experience for all primary situations.
