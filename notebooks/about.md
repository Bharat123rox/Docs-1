# About

## What is a Notebook?

Gradient notebooks are an interactive environment \(based on [Jupyter Notebook](https://jupyter.org/) or [Jupyter Lab](https://blog.jupyter.org/jupyterlab-is-ready-for-users-5a6f039b8906)\) for developing and running code. You can run Jupyter notebooks, Python scripts and much more, on a GPU, CPU, or even a TPU. A Gradient ****Notebook = access to a Jupyter Notebook instance. Within that instance you can have limitless notebook documents. You can think of a Gradient Notebook as your persistent, on-demand workspace in the cloud.

Within that instance you can have limitless notebook documents.

{% hint style="info" %}
**NEW!**  Visit the new [ML Showcase](https://ml-showcase.paperspace.com/) for a list of sample projects you can fork into your own account.
{% endhint %}

### File Storage

Any data stored in `/storage` will be preserved for you, across restarts. Persistent storage is backed by a filesystem and is ideal for storing data like images, datasets, model checkpoints etc.  Learn more about persistent storage [here](../data/storage.md#persistent-storage).

### Containers

Because everything is running in a Docker container behind the scenes, we support any kernel you would like. We have a handful of pre-built containers and you can also add a custom container very easily or build one off of a base template, such as the Jupyter R stack.

### Environment Variables

There are a number of environment variables loaded into a notebook's environment, which you can access and use. Probably most useful is is `PS_API_KEY` , which will contain your most recently created API key \(if you've created one\). In combination with the Gradient SDK, this allows you to easily, programmatically interact with Gradient.

